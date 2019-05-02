<template>
    <div class="has-text-centered">
        <div class="about">
            <figure class="image image is-128x128" style="margin:auto;">
                <img src="../assets/images/avatar.jpg" class="is-rounded">
            </figure>
            <p class="title is-size-3 has-text-weight-normal" style="margin:0.5rem;">Tirth Bal</p>
            <p class="heading is-size-6">Software Developer | Learner</p>
            <ul>
                <li>
                    <a href="https://github.com/tirthbal" target="_blank">
                        <i class="fab fa-github"></i>
                    </a>
                </li>
                <li>
                    <a href="https://twitter.com/tirth_bal" target="_blank">
                        <i class="fab fa-twitter"></i>
                    </a>
                </li>
                <li>
                    <a href="https://www.linkedin.com/in/tirthbal" target="_blank">
                        <i class="fab fa-linkedin"></i>
                    </a>
                </li>
                <li>
                    <a href="https://stackoverflow.com/users/5689871/sherlcode13" target="_blank">
                        <i class="fab fa-stack-overflow"></i>
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>
<script>
export default {
    name: "Home"
}
</script>
<style>
    .about li {
        display: inline;
        margin: auto 1rem;
    }
    .about li a {
        font-size:1.5rem;
        color: #363636;
    }
    .about li a:hover {
        color: #3273dc;
    }
</style>

