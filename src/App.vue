<template>
  <the-header title="Remember Me"></the-header>
  <stored-resources :resources="storedResources"></stored-resources>
</template>

<script>


import StoredResources from "@/components/learning-resources/StoredResources.vue";
import TheHeader from "@/components/layouts/TheHeader.vue";

export default {
  components: {TheHeader, StoredResources},
  data() {
    return {
      storedResources: [
        {
          id: 'official-guide',
          title: 'Official Guide',
          description: 'The official Vuw.js doc',
          link: 'https://vuw.js.org'
        },
        {
          id: 'google',
          title: 'Google',
          description: 'google doc',
          link: 'https://google.con'
        },
      ]
    }
  }
}
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

* {
  box-sizing: border-box;
}

html {
  font-family: 'Roboto', sans-serif;
}

body {
  margin: 0;
}
</style>
