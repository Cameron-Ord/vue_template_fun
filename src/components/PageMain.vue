<template>
        <section class="section_main">
            <article class="article_main">
                <variables-page></variables-page>
        
            </article>
        </section>
</template>

<script>
import variablesPage from './variablesPage.vue';
    export default {
        name: `blog_example`,

        components:{
          variablesPage

        }
    
    }
</script>

<style scoped>

.section_main{
    display: grid;

    align-items: center;

    justify-items: center;
}

.article_main{

    
}

</style>