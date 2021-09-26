<template>
    <div>
        <a href="https://www.facebook.com/Galatasaray/">
            <FontAwesomeIcon 
                :icon="['fab','facebook']" 
                class="menu-icon" 
                size="lg"
            />
        </a>
        <a href="https://twitter.com/GalatasaraySK">
            <FontAwesomeIcon 
                :icon="['fab','twitter']" 
                class="menu-icon" 
                size="lg"
        />
        </a>
        <a href="https://www.instagram.com/galatasaray/">
            <FontAwesomeIcon 
                :icon="['fab','instagram']" 
                class="menu-icon" 
                size="lg"
        />
        </a>
        <a href="https://www.youtube.com/user/2galatasaray">
            <FontAwesomeIcon 
                :icon="['fab','youtube']" 
                class="menu-icon" 
                size="lg"
            />
        </a>
    </div>
</template>

<style lang="postcss" scoped>
    .menu-icon {
        @apply text-yellow-500 cursor-pointer;
    }
</style>