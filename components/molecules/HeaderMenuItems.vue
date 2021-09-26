<template>
    <div>
        <a href="#" class="menu-title">GALATASARAY</a>
        <a href="#" class="menu-title">{{$t('header.football')}}</a>
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
        @apply text-yellow-500 text-xs cursor-pointer;
    }
</style>