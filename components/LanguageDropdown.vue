<template>
    <div class="dropdown" @click="toggleDropdown">
        <button class="dropdown__button" type="button">
                <span v-show="!showDropdown" class="dropdown__selected-language">{{selectedLanguage}}</span>
                <FontAwesomeIcon icon="chevron-down" size="lg"/>
        </button>
        <span v-show="showDropdown" class="dropdown__options">
            <nuxt-link :to="switchLocalePath('en')" class="dropdown__lang-option">
                <span>EN</span>
            </nuxt-link>
            <nuxt-link :to="switchLocalePath('tr')" class="dropdown__lang-option">
                <span>TR</span>
            </nuxt-link>
            <nuxt-link :to="switchLocalePath('fr')" class="dropdown__lang-option">
                <span>FR</span>
            </nuxt-link>
            <span class="py-2">
                <FontAwesomeIcon icon="chevron-up" size="lg"/>
            </span>
        </span>
    </div>
</template>

<script lang="ts">
import { defineComponent, ref, useContext, computed } from '@nuxtjs/composition-api'

export default defineComponent({
    setup() {
      const context = useContext();

      const showDropdown = ref(false);
      const selectedLanguage = computed(() => context.app.i18n.locale.toUpperCase());
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
        &__button {
            @apply flex flex-col items-center;
        }
        &__options {
            @apply top-2 w-14 bg-black absolute z-10 border border-t-0 border-gala-yellow flex flex-col items-center;
        }
        &__lang-option {
            @apply border-b border-gala-yellow hover:bg-gray-900 w-full text-center;
        }
        &__selected-language {
            @apply top-2 relative;
        }
    }
</style>
