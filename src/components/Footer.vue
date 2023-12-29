<script>
export default {
    name: "Footer"
}
</script>

<template>
    <footer>
        <div class="container">

            <div class="sing_up">
                <button>SING-UP NOW!</button>
            </div>

            <div class="follow_us">
                <h3>FOLLOW US</h3>
                <a href="#">
                    <img src="/imgs/footer-facebook.png" alt="facebbok">
                </a>
                <a href="#">
                    <img src="/imgs/footer-youtube.png" alt="youtube">
                </a>
                <a href="#">
                    <img src="/imgs/footer-twitter.png" alt="twitter">
                </a>
            </div>

        </div>
    </footer>
</template>

<style lang="scss" scoped>
// call variables
@use '../style/partials/variables' as *;
// call mixins
@use '../style/partials/mixins' as *;


footer {
    background-color: #303030;
}

.container {
    @include container;
    justify-content: space-between;
}

button {
    padding: 5px;
    border-color: #0582F9;
    background-color: #303030;
    color: white;
}

.follow_us {
    display: flex;
    align-items: center;
    gap: 10px;
}

h3 {
    color: $main-color;
}
</style>