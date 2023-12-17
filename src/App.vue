<template>
  <the-header title="Learning Resources"></the-header>
  <stored-resources :stored-resources="storedResources"></stored-resources>
</template>

<script>
import StoredResources from './components/learning-resources/StoredResources.vue';
import TheHeader from './components/layouts/TheHeader.vue';
export default {
  components: {
    StoredResources,
    TheHeader,
  },
  data() {
    return {
      storedResources: [
        {
          id: 1,
          title: 'Vue Documentation',
          link: 'https://vuejs.org',
          description: 'This is Vue documentation',
        },
        {
          id: 2,
          title: 'Google',
          link: 'https://google.com',
          description: 'This is google',
        },
        {
          id: 3,
          title: 'JavaScript',
          link: 'https://javascript.info/',
          description: 'Learn JavaScript',
        },
      ],
    };
  },
};
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
