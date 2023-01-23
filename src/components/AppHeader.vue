<script>
export default {
    name: 'AppHeader',
    props: {
        links: Array
    }
}
</script>

<template>
    <header>
        <div class="container">
            <figure>
                <img src="" alt="">
            </figure>

            <nav>
                <ul>
                    <li v-for="link in links" :key="link.text">{{ link.text }}</li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

header {
    height: $height-s;
    border: 2px solid red;
}
</style>