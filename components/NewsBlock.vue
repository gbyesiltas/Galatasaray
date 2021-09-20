<template>
    <div class="news-block">
        <div class="news-image"/>
        <div class="news-content">
            <div class="news-content-left">
                <h1 class="news-title">
                    SON DAKIKA
                </h1>
                <h1 class="news-title">
                    COK IYI BI SEYLER OLDU
                </h1>
            </div>
        </div>
    </div>
</template>

<style lang="postcss" scoped>
.news-image{
    @apply h-96 w-full bg-red-800;
    filter: grayscale(30%);
}
.news-content{
    @apply h-64 w-full bg-yellow-500 flex items-center;
    filter: grayscale(30%);
}
.news-content-left{
    @apply flex flex-col;
}
.news-title{
    @apply font-bold text-red-800 text-4xl ml-24;
}
</style>