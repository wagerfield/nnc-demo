<template>
  <div class="default-layout">
    <v-nav :links="links"/>
    <nuxt/>
  </div>
</template>

<script>
import VNav from "~/components/nav/nav.vue";

export default {
  data: () => ({
    links: [
      {
        path: "/",
        text: "Index"
      },
      {
        path: "/about",
        text: "About"
      },
      {
        path: "/broken",
        text: "Broken"
      }
    ]
  }),
  components: {
    VNav
  }
};
</script>

<style>
.default-layout {
  padding: 1rem;
  min-height: 100vh;
  box-sizing: border-box;
}
</style>
