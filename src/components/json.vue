<script setup>
import { ref } from "vue";

// Reactive variable to store Base64 encoded content for multiple files
const base64Files = ref([]);

// Handle multiple PDF file input and convert them to Base64
const handlePdfFileInput = (event) => {
  const files = event.target.files;
  base64Files.value = []; // Reset the array before processing new files

  Array.from(files).forEach((file) => {
    if (file && file.type === "application/pdf") {
      const reader = new FileReader();
      reader.onload = () => {
        const binaryString = reader.result;
        const base64Content = btoa(binaryString);

        // Push an object containing file details and Base64 content
        base64Files.value.push({
          filename: file.name,
          extension: "pdf",
          content: base64Content,
        });

        // Print the specific line with filename, extension, and content
        console.log({
          filename: file.name,
          extension: "pdf",
          content: base64Content,
        });

        // Also log the length of files array (which would be 1 or more depending on files selected)
        console.log("length:", base64Files.value.length);
      };
      // Read file as binary string
      reader.readAsBinaryString(file);
    } else {
      alert("Please select valid PDF files.");
    }
  });
};

// Upload the JSON object containing the Base64 data for multiple files
const uploadJson = async () => {
  if (base64Files.value.length === 0) {
    alert("Please select and encode PDF files first.");
    return;
  }

  // Create JSON object with an array of files
  const jsonData = {
    files: base64Files.value,
  };

  console.log("Uploading JSON:", jsonData);

  // Make a POST request to upload the JSON
  try {
    const response = await fetch("https://your-server-endpoint.com/upload", {
      method: "POST",
      headers: {
        "Content-Type": "application/json",
      },
      body: JSON.stringify(jsonData),
    });

    if (response.ok) {
      console.log("Files uploaded successfully");
    } else {
      console.error("Error uploading files:", response.statusText);
    }
  } catch (error) {
    console.error("Network error:", error);
  }
};
</script>

<template>
  <div>
    <input
      type="file"
      id="pdfFileInput"
      @change="handlePdfFileInput"
      accept="application/pdf"
      multiple
    />
    <button @click="uploadJson">Upload JSON</button>
    <div v-if="base64Files.length">
      <h3>Base64 Encoded Content:</h3>
      <ul>
        <li v-for="(file, index) in base64Files" :key="index">
          <h4>{{ file.filename }}</h4>
          <textarea
            :value="file.content"
            readonly
            rows="5"
            cols="50"
          ></textarea>
        </li>
      </ul>
    </div>
  </div>
</template>
