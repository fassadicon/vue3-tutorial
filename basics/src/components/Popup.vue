<template>
    <div>
        <h2>THis is a popup</h2>
        <input type="text" v-model="name">
        <button @click="$emit('xxx', name)">Close popup</button>
    </div>
</template>

<script>
    export default {
        name: "Popup",
        emits: {
            xxx: (name) => {
                return !name ? false : true;
            }
        },
        data() {
            return {
                name: ""
            }
        }
    }
</script>