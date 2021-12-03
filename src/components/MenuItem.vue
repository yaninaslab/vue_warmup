<template>
    <div class="menu_card">
        <img src="https://images.unsplash.com/photo-1638425793674-32119fffb3d5?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHwzMHx8fGVufDB8fHx8&auto=format&fit=crop&w=800&q=60" alt="">
        <h3>Food Ttile</h3>
        <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Labore, at?</p>
        <h5>Item Price</h5>

    </div>
</template>

<script>
    export default {
       name: "menu-item"
    }
</script>

<style scoped>
.menu_card {
    max-width: 300px;
    border-radius: 15px;
    box-shadow: 3px 3px 6px gray;
}
.menu_card > img {
    width: 270px;
    border-top-left-radius: 15px;
    border-top-right-radius: 15px;
}
</style>