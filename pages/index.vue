<template>
  <div>
    <Header />
    <NewsBlock />
    <Footer />
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

import Header from "../components/Header.vue";
import NewsBlock from "../components/NewsBlock.vue";
import Footer from "../components/Footer.vue";

export default Vue.extend({
  components: {
    Header,
    NewsBlock,
    Footer,
  }
})
</script>
