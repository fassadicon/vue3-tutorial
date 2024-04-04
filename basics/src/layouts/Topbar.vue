<template>
    <div>
        <h1>Hello {{ name }} aka {{ username }}</h1>
    </div>
</template>

<script>
export default {
    name: "Topbar",
    props: {
        name: String
    },
    inject: ["username"]
}
</script>