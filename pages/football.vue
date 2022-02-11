<template>
  <div class="football-content__container">
    <div>
      <h1 class="football-content__page-title">
        {{$t("header.football")}}
      </h1>
      <FootballCards />
    </div>
  </div>
</template>

<style lang="postcss" scoped>
.football-content {
  &__container {
    min-height: calc(100vh - 8rem);
    @apply w-full bg-gala-red px-28 py-20;
    filter: grayscale(30%);
  }
  &__page-title {
    @apply text-4xl font-bold text-gala-yellow;
  }
}
</style>
