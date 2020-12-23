<template>
    <header class="main-nav">
        <nuxt-link to="/" class="logo">TheKachi</nuxt-link>
        <nav class="main-nav__menu">         
            <ul class="nav__links">
                 <li tabindex="0"><toggle /></li>
                 <li><nuxt-link to="/background">Background</nuxt-link></li>
                <li><nuxt-link to="/projects">Projects</nuxt-link></li>
                <li><nuxt-link to="/contact">Contact</nuxt-link></li>
                <li class="btn"><nuxt-link to="/resume">Resume</nuxt-link></li>
               
            </ul>
            
        </nav>
    </header>
</template>

<script>
    import Toggle from './Toggle';
    export default {
        components: {
            Toggle
        },
        methods:{
            link(link){
            let deviceWidth = window.innerWidth;
            if(deviceWidth<900){
                document.getElementById('toggle').checked = false
                this.$router.push(link)
            }
            else{
                this.$router.push(link)
            }
        }
    }
};
</script>

<style>

</style>