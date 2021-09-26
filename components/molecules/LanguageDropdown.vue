<template>
    <button class="dropdown" @click="toggleDropdown">
        <div>
            <p v-show="!showDropdown" class="dropdown__selected-language">{{selectedLanguage}}</p>
            <FontAwesomeIcon icon="chevron-down" size="lg"/>
        </div>
        
        <div v-show="showDropdown" class="dropdown__options">
            <nuxt-link :to="switchLocalePath('en')" class="dropdown__lang-option">
                <p>EN</p>
            </nuxt-link>
            <nuxt-link :to="switchLocalePath('tr')" class="dropdown__lang-option">
                <p>TR</p>
            </nuxt-link>
            <nuxt-link :to="switchLocalePath('fr')" class="dropdown__lang-option">
                <p>FR</p>
            </nuxt-link>
            <div class="py-2">
                <FontAwesomeIcon icon="chevron-up" size="lg"/>
            </div>
        </div>
        
    </button>
</template>

<script lang="ts">
import { defineComponent, ref, useContext } from '@nuxtjs/composition-api'

export default defineComponent({
    setup() {
      const context = useContext();

      const showDropdown = ref(false);
      const selectedLanguage = ref(context.app.i18n.locale.toUpperCase());
      const toggleDropdown = () => {
          showDropdown.value = !showDropdown.value;
      };
      return {
          selectedLanguage,
          showDropdown,
          toggleDropdown,
      }
    },
})
</script>

<style lang="postcss" scoped>
    .dropdown {
        @apply flex flex-col items-center;
        &__options {
            @apply top-2 w-14 bg-black absolute z-10 border border-t-0 border-yellow-500 flex flex-col items-center;
        }
        &__lang-option {
            @apply border-b border-yellow-500 hover:bg-gray-500 w-full;
        }
        &__selected-language {
            @apply top-2 relative;
        }
    }
</style>
