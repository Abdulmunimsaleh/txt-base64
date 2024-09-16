<script setup>
import { ref } from "vue";

// Define reactive variables
const base64Encoded = ref("");
const postData = ref({
  data: [
    {
      filename: "RAG.pdf",
      extension: "pdf",
      content: "",
    },
  ],
});

// Handle text file input and convert to Base64
const handleTextFileInput = (event) => {
  const file = event.target.files[0];
  if (file) {
    const reader = new FileReader();
    reader.onload = () => {
      const textContent = reader.result;
      // Convert text content to Base64
      base64Encoded.value = btoa(textContent);
      console.log(base64Encoded);

      // Set the content in the JSON data structure
      postData.value.data[0].content = base64Encoded.value;

      console.log("JSON Data:", JSON.stringify(postData.value, null, 2));
    };
    reader.readAsText(file);
  }
};

// Function to trigger file reading and Base64 conversion
const submitFile = () => {
  const inputElement = document.getElementById("textFileInput");
  if (inputElement && inputElement.files.length > 0) {
    handleTextFileInput({ target: inputElement });
  }
};
</script>

<template>
  <div>
    <input type="file" id="textFileInput" @change="handleTextFileInput" />
    <button @click="submitFile">Submit</button>
  </div>
</template>
