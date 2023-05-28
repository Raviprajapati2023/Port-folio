<template>
  <HeaderApp />
  <slot />
  <router-view />
  <AppFooter />
</template>

<script>
import { defineComponent } from "vue";
import AppFooter from "./components/AppFooter.vue";
import HeaderApp from "./components/HeaderApp.vue";

export default defineComponent({
  name: "App",
  components: { AppFooter, HeaderApp },
});
</script>
