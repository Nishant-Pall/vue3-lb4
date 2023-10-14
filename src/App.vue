<template>
  <NavigationDrawer @change-page="changePage"></NavigationDrawer>
  <component :is="componentMap[currentComponent.componentName]"> </component>
</template>

<script setup>
import HomePage from "./components/HomePage.vue";
import HelloWorld from "./components/HelloWorld.vue";
import NavigationDrawer from "./components/NavigationDrawer.vue";
import { reactive, ref } from "vue";

const componentMap = {
  page_1: HomePage,
  page_2: HelloWorld,
  page_3: HomePage,
};

const currentComponent = ref({
  componentName: "page_1",
});

const changePage = (pageId) => {
  currentComponent.value.componentName = pageId;
};
</script>

<style scoped></style>
