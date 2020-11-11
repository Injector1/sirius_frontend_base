<template>
    <div id="app" class="container">
        <div class="row justify-content-md-center">
            <NameSurname class="col-lg" id="name-surname"/>
            <logo class="col-lg" id="logo"/>
        </div>
        <div class="row">
            <icon class="col" id="icon"/>
        </div>
    </div>
</template>

<script>
    import NameSurname from "./components/NameSurname";
    import Logo from "./components/Logo";
    import Icon from "./components/Icon";

    export default {
        name: 'App',
        components: {
            Icon,
            Logo,
            NameSurname
        }
    }
</script>

<style lang="scss">

    #app {
        margin-top: 10vh;
    }

    @media screen and (max-width: 990px) {
        #app {
            margin: auto;
            position: absolute;
            top: 50%;
            transform: translate(0, -50%)
        }
        #logo {
            order: 1;
            margin-bottom: 5%;
        }
        #name-surname {
            order: 2;
            margin-bottom: 5%;
        }
        #icon {
            order: 3;
            margin-bottom: 5%;
        }
    }
</style>
