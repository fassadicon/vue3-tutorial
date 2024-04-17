<template>
  <Topbar :name />
  <Home />
  <button @click="showPopup = true">Show Popup</button>

  <Input v-model="name" />
</template>

<script>
import Home from "./views/Home.vue";
import Topbar from "./layouts/Topbar.vue";
import Input from "./components/Input.vue";

export default {
  name: "App",
  components: {
    Topbar,
    Home,
    Input
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
