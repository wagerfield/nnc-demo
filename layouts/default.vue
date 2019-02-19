<template>
  <div>
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
