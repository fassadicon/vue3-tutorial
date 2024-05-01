<template>
  <Topbar :name />
  <PostList />
</template>

<script>
import Topbar from "./layouts/Topbar.vue";
import PostList from "./components/PostList.vue";

export default {
  name: "App",
  components: {
    Topbar,
    PostList
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
