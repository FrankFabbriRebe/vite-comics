<script>
export default {
    name: "Icons",

    data() {
        return {

            icons: [

                {
                    img: "/imgs/buy-comics-digital-comics.png",
                    text: "DIGITAL COMICS"
                },

                {
                    img: "/imgs/buy-comics-merchandise.png",
                    text: "DC MERCHANDISE"
                },

                {
                    img: "/imgs/buy-comics-subscriptions.png",
                    text: "SUBSCRIPTION"
                },

                {
                    img: "/imgs/buy-comics-shop-locator.png",
                    text: "COMIC SHOP LOCATOR"
                },

            ]

        }
    }

}
</script>

<template>
    <div class="icons">
        <div class="container">
            <div class="icon" v-for="icon in icons">
                <img :src="icon.img" :alt="icon.text">
                <span>{{ icon.text }}</span>
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
// call variables
@use '../style/partials/variables' as *;

.icons {
    background-color: $main-color;
}

.container {
    padding: 10px 50px;
    display: flex;
    justify-content: center;
}

.icon {
    display: flex;
    color: white;
    align-items: center;
    gap: 5px;
    margin: 10px;
}
</style>