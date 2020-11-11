<template>
    <div>
        <img src="../assets/icon.png"/>
    </div>
</template>

<script>
    export default {
        name: "Icon"
    }
</script>

<style scoped lang="scss">
    $size-desktop: 128px;
    $size-mobile: 100px;
    
    div {
        text-align: left;
        animation-name: fly;
        animation-duration: 2s;
        animation-iteration-count: infinite;

        img {
            width: $size-desktop;
            height: $size-desktop;
        }
    }
    
    @keyframes fly {
        0% {left: 0px}
        25% {left: 20px}
        75% {left: -20px}
        100% {left: 0px}
    }
    @media screen and (max-width: 990px) {
        div {
            img {
                width: $size-mobile;
                height: $size-mobile;
            }
        }
    }

    @media screen and (max-width: 1100px) {
        div {
            text-align: center;
        }
    }
</style>