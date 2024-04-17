<template>
    <div>
        <Article id="article_1" title="Article_1" :content="'This is a sample content'" :likes="50"/>
    </div>
    <div>
        <Card>Uwu</Card>
        <Card></Card>
    </div>
</template>

<script>
import Article from "../components/Article.vue";
import Card from "../components/Card.vue";

export default {
    name: "Home",
    components: {
        Article,
        Card
    }
}
</script>