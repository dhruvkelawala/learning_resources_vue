<template>
  <stored-resources :resources="storedResources"></stored-resources>
</template>

<script>
import StoredResources from "./components/learning-resources/StoredResources";

export default {
  components: {
    StoredResources,
  },
  data() {
    return {
      storedResources: [
        {
          id: "official-guide",
          title: "Official Guide",
          description: "The Official Vue.js documentation",
          link: "https://v3.vuejs.com",
        },
        {
          id: "google",
          title: "Google",
          description: "Learn to google...",
          link: "https://www.google.com",
        },
      ],
    };
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap");

* {
  box-sizing: border-box;
}

html {
  font-family: "Roboto", sans-serif;
}

body {
  margin: 0;
}
</style>