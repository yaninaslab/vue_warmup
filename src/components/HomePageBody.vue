<template>
    <div>
<h1 @click="make_blue">Welcome to the page!</h1>
<menu-item v-for="item in items" :key="item['title']" 
:price="item['price']" 
:title="item['title']" 
:description="item['desc']" 
:image_src="item['image_src']">
</menu-item>

<page-footer footer_title="I am Footer" copyrights="2021"></page-footer>
    </div>
</template>

<script>
import MenuItem from './MenuItem.vue';
import PageFooter from './PageFooter.vue';
    export default {
        name: "home-page-body",
        components: {
            MenuItem,
            PageFooter
        },

        methods: {
            make_blue() {
                document.body.style.background = "skyblue";

            },

        },


        data() {
            return {
                page_title: "Welcome to the page with many items!",
            items: [
                {
                    image_src: "https://images.unsplash.com/photo-1638425793674-32119fffb3d5?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHwzMHx8fGVufDB8fHx8&auto=format&fit=crop&w=800&q=60",
                    title: "Item Title 1",
                    desc: "Ths is a description",
                    price: 10.50
                },
                {
                    image_src: "https://images.unsplash.com/photo-1638425793674-32119fffb3d5?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHwzMHx8fGVufDB8fHx8&auto=format&fit=crop&w=800&q=60",
                    title: "Item Title 2",
                    desc: "Ths is a description",
                    price: 10.50
                },
                {
                    image_src: "https://images.unsplash.com/photo-1638425793674-32119fffb3d5?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxlZGl0b3JpYWwtZmVlZHwzMHx8fGVufDB8fHx8&auto=format&fit=crop&w=800&q=60",
                    title: "Item Title 3",
                    desc: "Ths is a description",
                    price: 10.50
                }
            ]
        }
        }
    }
</script>

<style scoped>

</style>