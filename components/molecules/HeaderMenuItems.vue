<template>
    <div>
        <NuxtLink :to="`/`" class="menu-title">GALATASARAY </NuxtLink>
        <NuxtLink :to="'/football'" class="menu-title">{{$t('header.football')}}</NuxtLink>
        <a href="#" class="menu-title">{{$t('header.basketball')}}</a>
        <a href="#" class="menu-title">{{$t('header.volleyball')}}</a>
        <a href="#" class="menu-title">{{$t('header.branches')}}</a>
        <a href="#" class="menu-title">{{$t('header.facilities')}}</a>
        <a href="#" class="menu-title">GSSTORE</a>
        <a href="#" class="menu-title">{{$t('header.history')}}</a>
    </div>
</template>

<style lang="postcss" scoped>
    .menu-title {
        @apply text-gala-yellow text-xs cursor-pointer py-4 px-2 hover:bg-gray-900;
    }
</style>