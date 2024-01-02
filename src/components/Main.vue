<script>
import Card from './Card.vue';

export default {
    name: "Main",

    components: {
        Card,
    }

}
</script>

<template>
    <main>
        <div class="jumbotron">

        </div>

        <div class="container">

            <card />

        </div>
    </main>
</template>

<style lang="scss" scoped>
// call mixins
@use '../style/partials/mixins' as *;

main {
    background-color: black;
    color: white;

}

.container {
    @include container;
}

.jumbotron {
    background-image: url('/imgs/jumbotron.jpg');
    background-size: cover;
    width: 100%;
    height: 300px;
}
</style>
