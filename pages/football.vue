<template>
  <div class="football-content__container"></div>
</template>

<script lang="ts">
import Vue from 'vue'

import Header from "../components/Header.vue";
import Footer from "../components/Footer.vue";

export default Vue.extend({
  components: {
    Header,
    Footer,
  }
})
</script>

<style lang="postcss" scoped>
.football-content {
  &__container {
    min-height: calc(100vh - 8rem);
    @apply w-full bg-gala-red;
    filter: grayscale(30%);
  }
}
</style>
