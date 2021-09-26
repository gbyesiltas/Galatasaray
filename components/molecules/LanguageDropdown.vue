<template>
    <button class="dropdown" @click="toggleDropdown">
        <div>
            <p v-show="!showDropdown" class="">EN</p>
            <FontAwesomeIcon icon="chevron-down" size="lg"/>
        </div>
        
        <div v-show="showDropdown" class="dropdown__options">
            <div class="dropdown__lang-option">
                <p>EN</p>
            </div>
            <div class="dropdown__lang-option">
                <p>TR</p>
            </div>
            <div class="dropdown__lang-option">
                <p>FR</p>
            </div>
            <FontAwesomeIcon icon="chevron-up" size="lg"/>
        </div>
        
    </button>
</template>

<script lang="ts">
import { defineComponent, ref } from '@nuxtjs/composition-api'

export default defineComponent({
    setup() {
    console.log("something");
      const showDropdown = ref(false);
      const toggleDropdown = () => {
          showDropdown.value = !showDropdown.value;
      };
      return {
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
            @apply w-12 bg-black absolute z-10 border border-yellow-500;
        }
        &__lang-option {
            @apply border-b border-yellow-500;
        }
    }
</style>
