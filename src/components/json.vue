<script setup>
import { ref } from "vue";

// Reactive variable to store Base64 encoded content
const base64Encoded = ref("");

// Handle PDF file input and convert it to Base64
const handlePdfFileInput = (event) => {
  const file = event.target.files[0];
  if (file && file.type === "application/pdf") {
    const reader = new FileReader();
    reader.onload = () => {
      const binaryString = reader.result;
      // Convert binary content to Base64
      base64Encoded.value = btoa(binaryString);

      console.log("Base64 Encoded PDF:", base64Encoded.value);
    };
    // Read file as binary string
    reader.readAsBinaryString(file);
  } else {
    alert("Please select a valid PDF file.");
  }
};

// Upload the JSON object containing the Base64 data
const uploadJson = async () => {
  if (!base64Encoded.value) {
    alert("Please select and encode a PDF file first.");
    return;
  }

  // Create JSON object with file details and Base64 content
  const jsonData = {
    filename: "RAG.pdf",
    extension: "pdf",
    content: base64Encoded.value,
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
      console.log("File uploaded successfully");
    } else {
      console.error("Error uploading file:", response.statusText);
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
    />
    <button @click="uploadJson">Upload JSON</button>
    <div v-if="base64Encoded">
      <h3>Base64 Encoded Content:</h3>
      <textarea :value="base64Encoded" readonly rows="10" cols="50"></textarea>
    </div>
  </div>
</template>
