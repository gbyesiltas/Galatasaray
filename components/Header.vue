<template>
    <div class="header">
        <img src="../assets/gala-logo.png" class="header__gala-logo"/>
        <div class="header__menu-sections">
            <div class="header__menu-section">
                <a href="#" class="header__menu-item">gs tv</a>
                <div class="header__seperator-line"></div>
                <div class="header__menu-section">
                    <FontAwesomeIcon :icon="['fab','facebook']" class="header__menu-item"/>
                    <a href="#" class="header__menu-item">twitter</a>
                    <a href="#" class="header__menu-item">instagram</a>
                    <a href="#" class="header__menu-item">youtube</a>
                </div>
                <div class="header__seperator-line"></div>
                <a href="#" class="header__menu-item">TR</a>
            </div>
            <div class="header__menu-section">
                <a href="#" class="header__menu-item">GALATASARAY SK</a>
                <a href="#" class="header__menu-item">FUTBOL</a>
                <a href="#" class="header__menu-item">BASKETBOL</a>
                <a href="#" class="header__menu-item">VOLEYBOL</a>
                <a href="#" class="header__menu-item">BRANSLAR</a>
                <a href="#" class="header__menu-item">TESISLER</a>
                <a href="#" class="header__menu-item">GSSTORE</a>
                <a href="#" class="header__menu-item">TARIHCE</a>
            </div>
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
    &__menu-item {
        @apply text-yellow-500 text-xs hover:bg-gray-900 px-2 py-4;
    }
    &__seperator-line {
        @apply w-px h-8 bg-yellow-500;
    }
}

</style>