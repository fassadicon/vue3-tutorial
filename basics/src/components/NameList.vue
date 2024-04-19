<template>
    <h3 v-for="name in names" :key="name.firstName">
        <slot :firstName="name.firstName" :lastName="name.lastName"></slot>
    </h3>
</template>

<script>
export default {
    name: "NameList",
    data() {
        return {
            names: [
                {
                    firstName: "John",
                    lastName: "Doe"
                },
                {
                    firstName: "Jam",
                    lastName: "Greed"
                },
                {
                    firstName: "John",
                    lastName: "Smith"
                }
            ]
        }
    }
}
</script>

<style scoped></style>