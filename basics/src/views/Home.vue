<template>
    <div>
        <Article id="article_1" title="Article_1" :content="'This is a sample content'" :likes="50"/>
    </div>
    <div>
        <Card>
            <template v-slot:header>Header</template>
            <template v-slot:default>Content</template>
            <template v-slot:footer>
                <a href="">Click here for more info</a>
            </template>
        </Card>
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