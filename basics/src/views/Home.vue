<template>
    <div>
        <Article id="article_1" title="Article_1" :content="'This is a sample content'" :likes="50"/>
    </div>
</template>

<script>
import Article from "../components/Article.vue";

export default {
    name: "Home",
    components: {
        Article
    }
}
</script>