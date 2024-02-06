<script>
// script setup
// import HelloWorld from "./components/HelloWorld.vue";
// import TheWelcome from "./components/TheWelcome.vue";
export default {
  name: "App",
  data() {
    return {
      names: ['Frans', 'Audrey', 'Segovia', 'Sadicon'],
      fullNames: [
        { first: "Frans", last: "Sadicon" },
        { first: "Carl", last: "Labado" },
        { first: "Jolina", last: "Sants" },
      ],
    };
  },
};
</script>

<template>
  <ul>
    <li v-for="name in fullNames">{{ name.first }} {{ name.last }}</li>
  </ul>
</template>

<!-- <style scoped>
.underlined {
  text-decoration: underline;
}

.lined-through {
  text-decoration: line-through;
}

.yellow {
  color: yellow;
}

/* header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
} */
</style> -->
