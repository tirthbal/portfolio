<template>
    <div id="app" style="margin-top:0;">
        <section class="hero is-fullheight" style="margin-top:0; ">
            <div class="hero-head">
            <navbar></navbar>
            <!-- header component  -->
            </div>
            <div class="hero-body">
                <div class="container">
                    <transition name="moveInUp">
                    <router-view></router-view>
                    </transition>
                </div>
            </div>
            <div class="hero-foot" style="margin-bottom: 5px;">
                <div class="content has-text-centered">
                    <p>&#169; 2019 | <a href="https://tirthbal.in">Tirth Bal</a> | <a href="http://creativecommons.org/licenses/by-nc-sa/4.0/">CC BY NC SA 4.0</a> |
                    Inspired from <a href="https://themes.gohugo.io/hugo-coder/">Hugo Coder Theme</a> | <br> Powered by Vue and Bulma | Made with &#9829;
                    </p>
                </div>
            </div>
        </section>
    </div>
</template>
<style lang="css">
    @import "../node_modules/bulma/css/bulma.css";
    .moveInUp-enter-active{
        animation: fadeIn 2s ease-in;
    }
    @keyframes fadeIn{
        0%{
            opacity: 0;
        }
        50%{
            opacity: 0.5;
        }
        100%{
            opacity: 1;
        }
    }
    .moveInUp-leave-active{
        animation: moveInUp .3s ease-in;
    }
    @keyframes moveInUp{
        0%{
            transform: translateY(0);
        }
        100%{
            transform: translateY(-400px);
        }
    }
</style>
<script>
    import Navbar from "./components/Header.vue";

    export default {
        name: "app",
        components: {
            Navbar
        }
    };
</script>

