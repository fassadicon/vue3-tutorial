<template>
    <div>
        <button @click="getPosts">Load Posts</button>
        <div v-for="post in posts" :key="post.id">
            <h2>{{ post.title }}</h2>
            <p>{{ post.body }}</p>
        </div>
    </div>
</template>

<script>
import axios from 'axios';
export default {
    name: 'PostList',
    data() {
        return {
            posts: []
        }
    },
    methods: {
        getPosts() {
            axios.get('https://jsonplaceholder.typicode.com/posts')
                .then(response => {
                    this.posts = response.data;
                })
                .catch(error => {
                    console.log(error);
                });
        }
    }
}
</script>

<style scoped>
</style>