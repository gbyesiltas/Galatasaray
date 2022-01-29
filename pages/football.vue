<template>
  <div class="bg-black">
    <Header />
    <div class="football-content">
        <h1>Football</h1>
    </div>
    <Footer />
  </div>
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
    min-height: calc(100vh - 8rem);
    @apply w-full bg-gala-red;
}
</style>
