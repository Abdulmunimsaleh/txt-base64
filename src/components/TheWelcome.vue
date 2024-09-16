<!-- <script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Documentation</template>

    Vue’s
    <a href="https://vuejs.org/" target="_blank" rel="noopener">official documentation</a>
    provides you with all information you need to get started.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>Tooling</template>

    This project is served and bundled with
    <a href="https://vitejs.dev/guide/features.html" target="_blank" rel="noopener">Vite</a>. The
    recommended IDE setup is
    <a href="https://code.visualstudio.com/" target="_blank" rel="noopener">VSCode</a> +
    <a href="https://github.com/johnsoncodehk/volar" target="_blank" rel="noopener">Volar</a>. If
    you need to test your components and web pages, check out
    <a href="https://www.cypress.io/" target="_blank" rel="noopener">Cypress</a> and
    <a href="https://on.cypress.io/component" target="_blank" rel="noopener"
      >Cypress Component Testing</a
    >.

    <br />

    More instructions are available in <code>README.md</code>.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>Ecosystem</template>

    Get official tools and libraries for your project:
    <a href="https://pinia.vuejs.org/" target="_blank" rel="noopener">Pinia</a>,
    <a href="https://router.vuejs.org/" target="_blank" rel="noopener">Vue Router</a>,
    <a href="https://test-utils.vuejs.org/" target="_blank" rel="noopener">Vue Test Utils</a>, and
    <a href="https://github.com/vuejs/devtools" target="_blank" rel="noopener">Vue Dev Tools</a>. If
    you need more resources, we suggest paying
    <a href="https://github.com/vuejs/awesome-vue" target="_blank" rel="noopener">Awesome Vue</a>
    a visit.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <CommunityIcon />
    </template>
    <template #heading>Community</template>

    Got stuck? Ask your question on
    <a href="https://chat.vuejs.org" target="_blank" rel="noopener">Vue Land</a>, our official
    Discord server, or
    <a href="https://stackoverflow.com/questions/tagged/vue.js" target="_blank" rel="noopener"
      >StackOverflow</a
    >. You should also subscribe to
    <a href="https://news.vuejs.org" target="_blank" rel="noopener">our mailing list</a> and follow
    the official
    <a href="https://twitter.com/vuejs" target="_blank" rel="noopener">@vuejs</a>
    twitter account for latest news in the Vue world.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading>Support Vue</template>

    As an independent project, Vue relies on community backing for its sustainability. You can help
    us by
    <a href="https://vuejs.org/sponsor/" target="_blank" rel="noopener">becoming a sponsor</a>.
  </WelcomeItem>
</template> -->
<!-- 
<script setup>
import { ref } from "vue";

// Define reactive variables
const base64Encoded = ref("");
const decodedContent = ref("");

// Handle text file input and convert to Base64
const handleTextFileInput = (event) => {
  const file = event.target.files[0];
  if (file) {
    const reader = new FileReader();
    reader.onload = () => {
      const textContent = reader.result;
      // Convert text content to Base64
      base64Encoded.value = btoa(textContent);
    };
    reader.readAsText(file);
  }
};

// Handle Base64 file input and decode back to text
const handleBase64FileInput = (event) => {
  const file = event.target.files[0];
  if (file) {
    const reader = new FileReader();
    reader.onload = () => {
      const base64String = reader.result;
      const base64Content = base64String.toString();
      // Decode Base64 back to text
      decodedContent.value = atob(base64Content);
    };
    reader.readAsText(file);
  }
};

// Trigger the conversion to Base64
const convertToBase64 = () => {
  const inputElement = document.getElementById("textFileInput");
  if (inputElement.files.length > 0) {
    handleTextFileInput({ target: { files: inputElement.files } });
  }
};

// Trigger the decoding from Base64
const decodeFromBase64 = () => {
  const inputElement = document.getElementById("base64FileInput");
  if (inputElement.files.length > 0) {
    handleBase64FileInput({ target: { files: inputElement.files } });
  }
};
</script>

<template>
  <div class="container">
    <h2 class="text-center">File Conversion Tool</h2>

    <!-- Input for selecting a text file -->
    <div class="mb-3">
      <label for="textFileInput" class="form-label"
        >Upload a Text File to Convert to Base64:</label
      >
      <input
        type="file"
        id="textFileInput"
        class="form-control"
        accept=".txt"
      />
    </div>

    <!-- Button to convert text file to Base64 -->
    <div class="mb-3">
      <button class="btn custom-btn" @click="convertToBase64">
        Convert to Base64
      </button>
    </div>

    <!-- Display the Base64 encoded content -->
    <div class="mb-3">
      <label for="base64Output" class="form-label">Base64 Encoded:</label>
      <textarea
        id="base64Output"
        class="form-control"
        rows="5"
        v-model="base64Encoded"
        readonly
      ></textarea>
    </div>

    <!-- Input for selecting a Base64 file -->
    <div class="mb-3">
      <label for="base64FileInput" class="form-label"
        >Upload a Base64 File to Convert to Text:</label
      >
      <input
        type="file"
        id="base64FileInput"
        class="form-control"
        accept=".txt"
      />
    </div>

    <!-- Button to decode Base64 file back to text -->
    <div class="mb-3">
      <button class="btn custom-btn" @click="decodeFromBase64">
        Decode from Base64
      </button>
    </div>

    <!-- Display the decoded content -->
    <div class="mb-3">
      <label for="decodedOutput" class="form-label">Decoded Content:</label>
      <textarea
        id="decodedOutput"
        class="form-control"
        rows="5"
        v-model="decodedContent"
        readonly
      ></textarea>
    </div>
  </div>
</template>

<style scoped>
.container {
  margin-top: 2rem;
  max-width: 600px;
}

.custom-btn {
  background-color: #007bff; /* Bootstrap primary color */
  color: white;
  border: none;
  width: 100%; /* Full width */
  padding: 0.5rem;
  border-radius: 0.25rem;
  font-size: 1rem;
}

.custom-btn:hover {
  background-color: #0056b3; /* Darker shade for hover effect */
  cursor: pointer;
}

.custom-btn:focus {
  box-shadow: 0 0 0 0.2rem rgba(38, 143, 255, 0.5); /* Focus outline */
}
</style> -->
