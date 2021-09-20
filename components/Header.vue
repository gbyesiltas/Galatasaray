<template>
    <div class="header">
        <img src="../assets/gala-logo.png" class="gala-logo"/>
        <div class="menu-sections">
            <div class="menu-section">
                <a href="#" class="menu-item">gs tv</a>
                <div class="seperator-line"></div>
                <div class="menu-section">
                    <a href="#" class="menu-item">facebook</a>
                    <a href="#" class="menu-item">twitter</a>
                    <a href="#" class="menu-item">instagram</a>
                    <a href="#" class="menu-item">youtube</a>
                </div>
                <div class="seperator-line"></div>
                <a href="#" class="menu-item">TR</a>
            </div>
            <div class="menu-section">
                <a href="#" class="menu-item">GALATASARAY SK</a>
                <a href="#" class="menu-item">FUTBOL</a>
                <a href="#" class="menu-item">BASKETBOL</a>
                <a href="#" class="menu-item">VOLEYBOL</a>
                <a href="#" class="menu-item">BRANSLAR</a>
                <a href="#" class="menu-item">TESISLER</a>
                <a href="#" class="menu-item">GSSTORE</a>
                <a href="#" class="menu-item">TARIHCE</a>
            </div>
        </div>
    </div>
</template>

<style lang="postcss" scoped>
.header{
    @apply h-24 bg-black flex;
}

.gala-logo{
    @apply h-40 ml-16 z-10;
}

.menu-sections{
    @apply flex flex-col flex-1 items-end mr-16;
}

.menu-section{
    @apply flex space-x-4 relative h-full items-center;
}

.menu-item{
    @apply text-yellow-500 text-xs hover:bg-gray-900 px-2 py-4;
}

.seperator-line{
    @apply w-px h-8 bg-yellow-500;
}

</style>