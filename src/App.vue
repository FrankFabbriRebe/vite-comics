<script>
import Header from './components/Header.vue';
import Main from './components/Main.vue';
import Icons from './components/Icons.vue';
import Links from './components/Links.vue';
import Footer from './components/Footer.vue';




export default {
    components: {
        Header,
        Main,
        Icons,
        Links,
        Footer
    }
}
</script>

<template>
    <Header />
    <Main />
    <Icons />
    <Links />
    <Footer />
</template>

<style lang="scss">
// inclusion general.scss
@use "./style/general.scss"
</style>
