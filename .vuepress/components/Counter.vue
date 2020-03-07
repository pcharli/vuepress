<template>
    <div>
        <button @click="increment()">+</button>
        <strong>{{value}}</strong>
    </div>
</template>

<script>
export default {
    props: ['initValue'],
    data() {
        return {
            value: this.initValue
        }
    },
    methods: {
        increment() { this.value ++}
    }
}
</script>

<style lang="scss">
$color: green;
button {
    background-color: $color;
}
</style>