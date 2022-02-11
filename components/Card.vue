<template>
    <div class="card">
        <div v-if="cardImg" class="card__img__container">
            <img class="card__img" :src="cardImg" alt="football-squad-image" />
        </div>
        <div class="card__title__container">
            <h2 class="card__title">{{ cardTitle }}</h2>
        </div>
    </div>
</template>
<script>
import { defineComponent } from '@vue/composition-api'

export default defineComponent({
    props: {
        cardImg: {
            type: String,
            required: false,
            default: "",
        },
        cardTitle: {
            type: String,
            required: true,
        }
    }
})
</script>

<style lang="postcss" scoped>
    .card {
        @apply w-full h-96 bg-gala-yellow px-4 shadow-md cursor-pointer hover:shadow-2xl;
        &__img {
            @apply object-cover h-full w-full;
            &__container {
                @apply py-4 h-4/5;
            }
        }
        &__title {
            @apply text-2xl font-bold text-gala-red;
            &__container {}
        }
    }
</style>