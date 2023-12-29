<script>
export default {
    name: "Main"
}
</script>

<template>
    <main>
        <div class="container">
            <span>Content goes here</span>
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
</style>
