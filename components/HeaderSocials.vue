<template>
    <div>
        <a href="https://www.facebook.com/Galatasaray/" aria-label="facebook link" rel="noopener noreferrer" target="_blank">
            <FontAwesomeIcon 
                :icon="['fab','facebook']" 
                alt="facebook icon"
                class="menu-icon" 
                size="lg"
            />
        </a>
        <a href="https://twitter.com/GalatasaraySK" aria-label="twitter link" rel="noopener noreferrer" target="_blank">
            <FontAwesomeIcon 
                :icon="['fab','twitter']" 
                alt="twitter icon"
                class="menu-icon" 
                size="lg"
        />
        </a>
        <a href="https://www.instagram.com/galatasaray/" aria-label="instagram link" rel="noopener noreferrer" target="_blank">
            <FontAwesomeIcon 
                :icon="['fab','instagram']" 
                alt="instagram icon"
                class="menu-icon" 
                size="lg"
        />
        </a>
        <a href="https://www.youtube.com/user/2galatasaray" aria-label="youtube link" rel="noopener noreferrer" target="_blank">
            <FontAwesomeIcon 
                :icon="['fab','youtube']" 
                alt="youtube icon"
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