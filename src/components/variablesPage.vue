<template>
    <div>
        <button @click="hack_post">Click me</button>
        <h3>{{ blog_title }}</h3>
        <p>{{ blog_content }}</p>
        <img :src="blog_image_url" alt="blog image">
    </div>
</template>

<script>
export default {

    methods: {


        hack_post: function () {

            this.blog_content = this.blog_content + `I was injected`;

        }

    },


        data() {
            return {
                blog_title: `Cameron's Blog`,
           
                blog_content:`ETHICAL DILEMMA: both cats are meowing for you to come play with them but are in separate rooms and are watching you so they will know if you choose the other cat.`,

                blog_image_url: `https://images.unsplash.com/photo-1552058544-f2b08422138a?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxzZWFyY2h8Nnx8cGVyc29ufGVufDB8fDB8fA%3D%3D&auto=format&fit=crop&w=500&q=60`,
            }
        },


    }
</script>

<style scoped>

</style>