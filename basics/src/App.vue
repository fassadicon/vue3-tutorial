<template>
  <Topbar :name />
  <button @click="activeTab = 'TabA'">Tab A</button>
  <button @click="activeTab = 'TabB'">Tab B</button>
  <button @click="activeTab = 'TabC'">Tab C</button>

  <keep-alive>
    <component :is="activeTab"/>
  </keep-alive>
  <!-- <TabA v-if="activeTab === 'TabA'"></TabA>
  <TabB v-if="activeTab === 'TabB'"></TabB>
  <TabC v-if="activeTab === 'TabC'"></TabC> -->
</template>

<script>
import Topbar from "./layouts/Topbar.vue";
import TabA from "./components/TabA.vue";
import TabB from "./components/TabB.vue";
import TabC from "./components/TabC.vue";

export default {
  name: "App",
  components: {
    Topbar,
    TabA,
    TabB,
    TabC
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
