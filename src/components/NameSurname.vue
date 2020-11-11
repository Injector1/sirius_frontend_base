<template>
    <div>
        <h1>{{ fullName }}</h1>
    </div>
</template>

<script>
    export default {
        name: "NameSurname",
        data() {
            return {
                fullName: "Demyan Kurbatov"
            }
        }
    }
</script>

<style scoped lang="scss">
    $font-stack: -apple-system, sans-serif;
    $font-size-header-desktop: 64px;
    $font-size-header-mobile: 50px;

    div {
        text-align: center;
        margin: auto;

        h1 {
            font-family: $font-stack;
            font-size: $font-size-header-desktop;
            margin: 0;
            padding: 0;
        }
    }

    @media screen and (max-width: 990px) {
        div {
            h1 {
                font-size: $font-size-header-mobile;
            }
        }
    }
</style>