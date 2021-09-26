<template>
  <div class="bg-black">
    <Header />
    <HomeBanner />
    <Footer />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

import Header from "../components/Header.vue";
import HomeBanner from "../components/HomeBanner.vue";
import Footer from "../components/Footer.vue";

export default Vue.extend({
  components: {
    Header,
    HomeBanner,
    Footer,
  }
})
</script>
