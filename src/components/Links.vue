<script>
export default {
    name: "Links"
}
</script>

<template>
    <div class="links">
        <div class="container">
            <div class="col">

                <h3>DC COMICS</h3>
                <a href="#">Characters</a>
                <a href="#">Comics</a>
                <a href="#">Movies</a>
                <a href="#">TV</a>
                <a href="#">Games</a>
                <a href="#">Videos</a>
                <a href="#">News</a>

                <h3>SHOP</h3>
                <a href="#">Shop DC</a>
                <a href="#">Shop DC Collections</a>

            </div>

            <div class="col">

                <h3>DC</h3>
                <a href="#">News</a>
                <a href="#">News</a>
                <a href="#">News</a>
                <a href="#">News</a>
                <a href="#">News</a>
                <a href="#">News</a>
                <a href="#">News</a>
                <a href="#">News</a>
                <a href="#">News</a>
                <a href="#">News</a>
                <a href="#">News</a>

            </div>

            <div class="col">

                <h3>SITES</h3>
                <a href="#">DC</a>
                <a href="#">MAD magazine</a>
                <a href="#">DC Kids</a>
                <a href="#">DC Universe</a>

            </div>

        </div>
    </div>
</template>

<style lang="scss" scoped>
// call mixins
@use '../style/partials/mixins' as *;

.links {
    background-image: url('/imgs/footer-bg.jpg');
    color: white;

    a {
        color: grey;
        text-decoration: none;

    }

    h3 {
        margin-bottom: 10px;
        margin-top: 10px;
    }

}

.container {
    @include container;
    gap: 100px;
}

.col {
    display: flex;
    flex-direction: column;
}
</style>