<template>
    <div class="header">
        <img src="/gala-logo.png" alt="galatasaray logo" class="header__gala-logo"/>
        <div class="header__menu-sections">
            <div class="header__menu-section">
                <img src="/gstv.png" alt="gs tv logo" class="header__menu-icon w-10" />
                <div class="header__seperator-line"></div>
                <HeaderSocials class="header__menu-section" />
                <div class="header__seperator-line"></div>
                <div class="header__menu-icon">
                    <LanguageDropdown />
                </div>
            </div>
            <HeaderMenuItems class="header__menu-section" />
        </div>
    </div>
</template>

<style lang="postcss" scoped>
.header{
    @apply h-24 bg-black flex;
    &__gala-logo {
        @apply h-40 ml-16 z-10;
    }
    &__menu-sections {
        @apply flex flex-col flex-1 items-end mr-16;
    }
    &__menu-section {
        @apply flex space-x-4 relative h-full items-center;
    }
    &__menu-icon {
        @apply text-gala-yellow cursor-pointer;
    }
    &__seperator-line {
        @apply w-px h-8 bg-gala-yellow;
    }
}

</style>