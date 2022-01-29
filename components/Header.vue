<template>
    <div class="header">
        <nuxt-img src="/gala-logo.png" class="header__gala-logo"/>
        <div class="header__menu-sections">
            <div class="header__menu-section">
                <nuxt-img src="/gstv.png" class="header__menu-icon w-10" />
                <div class="header__seperator-line"></div>
                <HeaderSocials class="header__menu-section" />
                <div class="header__seperator-line"></div>
                <div href="#" class="header__menu-icon">
                    <LanguageDropdown />
                </div>
            </div>
            <HeaderMenuItems class="header__menu-section" />
        </div>
    </div>
</template>

<script>
import { defineComponent as dc } from '#imports'
import HeaderMenuItems from "~/components/molecules/HeaderMenuItems.vue";
import HeaderSocials from "~/components/molecules/HeaderSocials.vue";
import LanguageDropdown from "~/components/molecules/LanguageDropdown.vue";

export default dc({
    components: {
        HeaderMenuItems,
        HeaderSocials,
        LanguageDropdown,
    },
    setup() {
        
    },
})
</script>

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