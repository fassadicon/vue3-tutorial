<template>
    <div class="card">
        <slot>Default</slot>
    </div>
</template>

<script>
    export default {
        name: "Card"
    }
</script>

<style scoped>
.card {
    border: 3px solid red;
}
</style>