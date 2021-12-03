<template>
    <footer @click="make_purple">
<h1>{{ footer_title }}</h1>
<p>{{ copyrights }}</p>
    </footer>
</template>

<script>
    export default {
        name: "page-footer",
        props: {
            footer_title: String,
            copyrights: String
        },
        methods: {
            make_purple() {
                document.body.style.background = "purple";
            }
        }

    }
</script>

<style scoped>
footer {
    min-height: 10vh;
    background: white;
    display: grid;
    place-items: center;
}

</style>