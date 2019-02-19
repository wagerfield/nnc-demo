<template>
  <ul class="nav-list">
    <li class="nav-item" v-for="link in links" :key="link.path">
      <nuxt-link :to="link.path" v-text="link.text"/>
    </li>
  </ul>
</template>

<script>
export default {
  props: {
    links: Array
  }
};
</script>

<style lang="scss" src="./nav.scss"/>
