<script>
export default {
    name: "Header",

    data() {
        return {

            pages: [
                {
                    title: "CHARACTERS",
                    active: false,
                },
                {
                    title: "COMICS",
                    active: true,
                },
                {
                    title: "MOVIES",
                    active: false,
                },
                {
                    title: "TV",
                    active: false,
                },
                {
                    title: "GAMES",
                    active: false,
                },
                {
                    title: "COLLECTIONS",
                    active: false,
                },
                {
                    title: "VIDEOS",
                    active: false,
                },
                {
                    title: "FANS",
                    active: false,
                },
                {
                    title: "NEWS",
                    active: false,
                },
                {
                    title: "SHOP",
                    active: false,
                }
            ]

        }
    }
}
</script>

<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="/imgs/dc-logo.png" alt="dc-logo">
            </div>
            <div class="pages">
                <ul>
                    <li v-for="page in pages">
                        <a :class="page.active ? 'active' : ''" href="#">{{ page.title }}</a>
                    </li>
                </ul>
            </div>
        </div>
    </header>
</template>

<style lang="scss" scoped>
// call variables
@use '../style/partials/variables' as *;

.container {
    display: flex;
    align-items: center;
    padding: 10px 50px;
}

.logo {
    width: 50%;
}

ul {
    list-style-type: none;
    display: flex;
}

a {
    text-decoration: none;
    color: black;
    margin-right: 20px;
}

.active {
    color: $main-color;
}
</style>
