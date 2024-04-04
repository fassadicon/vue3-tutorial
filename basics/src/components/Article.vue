<template>
    <div>
        <h2 v-bind="$attrs">{{ title }}</h2>
        <p>{{ content }}</p>
        <p>Likes: {{ likes }}</p>
        <p>Comment as {{ username }}</p>
    </div>
</template>

<script>
export default {
    name: "Article",
    props: {
        title: {
            type: String,
            required: true,
            default: "No title"
        },
        content: String,
        likes: Number
    },
    inheritAttrs: false,
    inject: ["username"]
}
</script>