<template>
    <div class="banner__block">
        <div class="banner__background">
            <div class="banner__image-container">
            <img class="banner__image banner__image__hagi-uefa" src="/hagi-uefa.jpg" alt="hagi uefa" />
            <img class="banner__image banner__image__taylan" src="/taylan.jpg" alt="taylan antalyali" />
            <img class="banner__image banner__image__lise" src="/lise.jpg" alt="galatasaray lisesi" />
            </div>
        </div>
        <div class="banner__bottom">
            <div class="banner__bottom-left">
                <div class="banner__title">
                    FİKRİ HÜR
                </div>
                <div class="banner__title">
                    VİCDANI HÜR
                </div>
            </div>
        </div>
    </div>
</template>

<style lang="postcss" scoped>
.banner{
    &__background{
        @apply w-full bg-gala-red;
        height: 30rem;
        filter: grayscale(30%);
    }
    &__image-container{
        @apply pt-12 ml-8;
    }
    &__image {
        @apply relative w-96 float-left;
        filter: grayscale(30%);
        &__lise {
            @apply left-8 top-8;
        }
        &__taylan {
            @apply left-32 top-16 z-10;

        }
        &__hagi-uefa {
            @apply left-52 top-12;
        }
    }
    &__bottom{
        @apply h-64 w-full bg-gala-yellow flex items-center;
        filter: grayscale(30%);
    }
    &__bottom-left{
        @apply flex flex-col;
    }
    &__title{
        @apply font-bold text-gala-red text-4xl ml-24;
    }
}
</style>