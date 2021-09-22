<template>
    <div class="header">
        <img src="../assets/gala-logo.png" class="header__gala-logo"/>
        <div class="header__menu-sections">
            <div class="header__menu-section">
                <img src="../assets/gstv.png" class="header__menu-icon w-10" />
                <div class="header__seperator-line"></div>
                <div class="header__menu-section">
                    <a href="https://www.facebook.com/Galatasaray/">
                    <FontAwesomeIcon 
                        :icon="['fab','facebook']" 
                        class="header__menu-icon" 
                        size="lg"
                    />
                    </a>
                    <a href="https://twitter.com/GalatasaraySK">
                    <FontAwesomeIcon 
                        :icon="['fab','twitter']" 
                        class="header__menu-icon" 
                        size="lg"
                    />
                    </a>
                    <a href="https://www.instagram.com/galatasaray/">
                    <FontAwesomeIcon 
                        :icon="['fab','instagram']" 
                        class="header__menu-icon" 
                        size="lg"
                    />
                    </a>
                    <a href="https://www.youtube.com/user/2galatasaray">
                    <FontAwesomeIcon 
                        :icon="['fab','youtube']" 
                        class="header__menu-icon" 
                        size="lg"
                    />
                    </a>
                </div>
                <div class="header__seperator-line"></div>
                <a href="#" class="header__menu-icon">EN</a>
            </div>
            <div class="header__menu-section">
                <a href="#" class="header__menu-title">GALATASARAY</a>
                <a href="#" class="header__menu-title">{{$t('header.football')}}</a>
                <a href="#" class="header__menu-title">{{$t('header.basketball')}}</a>
                <a href="#" class="header__menu-title">{{$t('header.volleyball')}}</a>
                <a href="#" class="header__menu-title">{{$t('header.branches')}}</a>
                <a href="#" class="header__menu-title">{{$t('header.facilities')}}</a>
                <a href="#" class="header__menu-title">GSSTORE</a>
                <a href="#" class="header__menu-title">{{$t('header.history')}}</a>
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