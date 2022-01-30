<template>
    <div>
        <NuxtLink :to="`/`" class="menu-title">GALATASARAY </NuxtLink>
        <NuxtLink :to="'/football'" class="menu-title">{{$t('header.football')}}</NuxtLink>
        <NuxtLink :to="`/`" class="menu-title">{{$t('header.basketball')}}</NuxtLink>
        <NuxtLink :to="`/`" class="menu-title">{{$t('header.volleyball')}}</NuxtLink>
        <NuxtLink :to="`/`" class="menu-title">{{$t('header.branches')}}</NuxtLink>
        <NuxtLink :to="`/`" class="menu-title">{{$t('header.facilities')}}</NuxtLink>
        <NuxtLink :to="`/`" class="menu-title">GSSTORE</NuxtLink>
        <NuxtLink :to="`/`" class="menu-title">{{$t('header.history')}}</NuxtLink>
    </div>
</template>

<style lang="postcss" scoped>
    .menu-title {
        @apply text-gala-yellow text-xs cursor-pointer py-4 px-2 hover:bg-gray-900;
    }
</style>