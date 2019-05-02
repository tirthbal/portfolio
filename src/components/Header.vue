<template>
    <nav class="navbar">
        <div class="container">
            <div class="navbar-brand">
                <router-link tag="a" class="navbar-item is-size-5 has-text-weight-semibold"
                to="/" exact-active-class="is-active">Tirth Bal</router-link>
                <span class="navbar-burger burger" data-target="navbarMenuHeroA" @click="menuStateOpen = !menuStateOpen">
                    <span></span>
                    <span></span>
                    <span></span>
                </span>
            </div>
            <div id="navbarMenuHeroA" class="navbar-menu" :class="{'is-active': menuStateOpen}">
                <div class="navbar-end">
                    <router-link tag="a" class="navbar-item some-item" to="/" exact-active-class="is-active">Home</router-link>
                    <router-link tag="a" class="navbar-item some-item" to="/about" exact-active-class="is-active">About</router-link>
                    <!-- <router-link tag="a" class="navbar-item" to="/projects" active-class="is-active">Projects</router-link> -->
                </div>
            </div>
        </div>
    </nav>
</template>
<script>
export default {
    name: "navbar",
    data() {
        return {
            'menuStateOpen': false
        }
    }
};
</script>
<style>
    @media only screen and (min-width: 1216px) {
        .some-item {
            padding:0 !important;
            margin: 1rem !important;
            transition: 0.7s all !important;
        }
        .some-item.is-active {
            border-bottom: 2px solid;
        }
    }
</style>

