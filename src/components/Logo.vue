<template>
    <div>
        <img src="../assets/logo.png"/>
    </div>
</template>

<script>
    export default {
        name: "Logo"
    }
</script>

<style scoped lang="scss">
    $size-desktop: 128px;
    $size-mobile: 100px;

    div {
        text-align: center;

        img {
            width: $size-desktop;
            height: $size-desktop;
            border-radius: 50%;
        }
    }

    @media screen and (max-width: 990px) {
        div {
            img {
                width: $size-mobile;
                height: $size-mobile;
            }
        }
    }
</style>