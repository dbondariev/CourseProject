<template>
  <ul>
    <learning-resource
      v-for="resource in storedResources"
      :key="resource.id"
      :resource="resource"
      :title="resource.title"
      :link="resource.link"
      :description="resource.description"
    ></learning-resource>
  </ul>
</template>

<script>
import LearningResource from './components/learning-resources/LearningResource.vue';

export default {
  components: {
    LearningResource,
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
ul {
  list-style: none;
  padding: 0;
}
li {
  margin-bottom: 1rem;
}
h1 {
  margin-bottom: 0.5rem;
}
a {
  color: #42b983;
  text-decoration: none;
}
a:hover {
  text-decoration: underline;
}
p {
  margin: 0;
}
</style>
