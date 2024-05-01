<template>
  <Topbar :name />
  <teleport to="#portal-root">
    <Portal/>
  </teleport>
</template>

<script>
import Topbar from "./layouts/Topbar.vue";
import Portal from "./components/Portal.vue"

export default {
  name: "App",
  components: {
    Topbar,
    Portal
  },
  data() {
    return {
      name: "Juan",
      activeTab: "TabA"
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

<style scoped>
</style>
