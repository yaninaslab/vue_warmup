<template>
    <div class="menu_card" v-if="price < 100 && price > 1">
        <img src="https://images.unsplash.com/photo-1638425793674-32119fffb3d5?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHwzMHx8fGVufDB8fHx8&auto=format&fit=crop&w=800&q=60" alt="">
        <h3>{{ title }}</h3>
        <p>{{ description }}</p>
        <h5>{{ price }}</h5>

    </div>
    <div v-else>
        <H1>Invalid Price!</H1>

    </div>
</template>

<script>
    export default {
       name: "menu-item",
       mounted () {
           document.body.style.background = "orange";
       },
       props: {
           image_src: String,
           title: String,
           description: String,
           price: Number
       },
    }
</script>

<style scoped>

.menu_card {
    max-width: 300px;
    border-radius: 15px;
    box-shadow: 3px 3px 6px gray;
}
.menu_card > img {
    width: 250px;
    border-top-left-radius: 15px;
    border-top-right-radius: 15px;
}
</style>