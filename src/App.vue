<template>
  <h1>{{ greeting }}</h1>
</template>

<script>
export default {
  data() {
    return {
      greeting: 'Hello World!',
    };
  },
};
</script>

<style>
h1 {
  color: red;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 2rem;
  border: 1rem solid black;
  background-color: darkgray;
}
</style>
