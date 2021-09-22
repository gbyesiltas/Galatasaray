<template>
    <div class="header">
        <img src="../assets/gala-logo.png" class="header__gala-logo"/>
        <div class="header__menu-sections">
            <div class="header__menu-section">
                <img src="../assets/gstv.png" class="header__menu-icon w-10" />
                <div class="header__seperator-line"></div>
                <div class="header__menu-section">
                    <FontAwesomeIcon 
                        :icon="['fab','facebook']" 
                        class="header__menu-icon" 
                        size="lg"
                    />
                    <FontAwesomeIcon 
                        :icon="['fab','twitter']" 
                        class="header__menu-icon" 
                        size="lg"
                    />
                    <FontAwesomeIcon 
                        :icon="['fab','instagram']" 
                        class="header__menu-icon" 
                        size="lg"
                    />
                    <FontAwesomeIcon 
                        :icon="['fab','youtube']" 
                        class="header__menu-icon" 
                        size="lg"
                    />
                </div>
                <div class="header__seperator-line"></div>
                <a href="#" class="header__menu-icon">TR</a>
            </div>
            <div class="header__menu-section">
                <a href="#" class="header__menu-title">GALATASARAY SK</a>
                <a href="#" class="header__menu-title">FUTBOL</a>
                <a href="#" class="header__menu-title">BASKETBOL</a>
                <a href="#" class="header__menu-title">VOLEYBOL</a>
                <a href="#" class="header__menu-title">BRANSLAR</a>
                <a href="#" class="header__menu-title">TESISLER</a>
                <a href="#" class="header__menu-title">GSSTORE</a>
                <a href="#" class="header__menu-title">TARIHCE</a>
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
    &__menu-icon {
        @apply text-yellow-500 cursor-pointer;
    }
    &__menu-title {
        @apply text-yellow-500 text-xs cursor-pointer;
    }
    &__seperator-line {
        @apply w-px h-8 bg-yellow-500;
    }
}

</style>