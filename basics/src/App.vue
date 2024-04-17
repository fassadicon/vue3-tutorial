<template>
  <Topbar :name />
  <Home />
</template>

<script>
import Home from "./views/Home.vue";
import Topbar from "./layouts/Topbar.vue";

export default {
  name: "App",
  components: {
    Topbar,
    Home
  },
  data() {
    return {
      name: "",
    }
  },
  provide() {
    return {
      username: "JDC123"
    }
  },
  methods: {
  }
}
</script>
