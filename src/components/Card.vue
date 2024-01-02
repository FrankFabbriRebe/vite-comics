<script>
export default {
    name: "Card",
    props: {
        details: Object
    }
}
</script>

<template>
    <div class="card">
        <div class="cover">
            <img :src="details.thumb" alt="details.series">
        </div>
        <h3>{{ details.series }}</h3>
    </div>
</template>

<style lang="scss" scoped>
.card {
    width: calc(100% / 6 - 10px);
    margin-bottom: 30px;
    margin-top: 30px;

    .cover {
        background-color: green;
        width: 100%;
        height: 250px;
        margin-bottom: 10px;

        img {
            width: 100%;
            height: 100%;
        }
    }

}
</style>
