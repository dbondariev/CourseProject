<template>
  <li>
    <div>
      <header>
        <h3>{{ title }}</h3>
        <button>Delete</button>
      </header>
    </div>
    <p>{{ description }}</p>
    <nav>
      <a :href="link" target="_blank">View Resource</a>
    </nav>
  </li>
</template>

<script>
export default {
  props: ['title', 'link', 'description'],
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
</style>
