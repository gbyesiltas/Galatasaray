<template>
    <div>
        <a href="https://www.facebook.com/Galatasaray/" rel="noopener noreferrer" target="_blank">
            <FontAwesomeIcon 
                :icon="['fab','facebook']" 
                class="menu-icon" 
                size="lg"
            />
        </a>
        <a href="https://twitter.com/GalatasaraySK" rel="noopener noreferrer" target="_blank">
            <FontAwesomeIcon 
                :icon="['fab','twitter']" 
                class="menu-icon" 
                size="lg"
        />
        </a>
        <a href="https://www.instagram.com/galatasaray/" rel="noopener noreferrer" target="_blank">
            <FontAwesomeIcon 
                :icon="['fab','instagram']" 
                class="menu-icon" 
                size="lg"
        />
        </a>
        <a href="https://www.youtube.com/user/2galatasaray" rel="noopener noreferrer" target="_blank">
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
        @apply text-gala-yellow cursor-pointer;
    }
</style>