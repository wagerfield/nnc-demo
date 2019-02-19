<template>
  <div class="error-page">
    <h1 v-text="error.statusCode"/>
    <h2 v-text="error.message"/>
    <nuxt-link to="/">Take me home</nuxt-link>
  </div>
</template>

<script>
export default {
  layout: "blank",
  props: {
    error: Object
  }
};
</script>

<style lang="scss">
.error-page {
  padding: 1rem;
  min-height: 100vh;
  box-sizing: border-box;
  background-color: red;
}
</style>
