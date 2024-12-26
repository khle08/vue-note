<template>
    <button v-on:click="changeView(1)">single</button>
    <button @click="changeView(2)">double</button>
    <div class="container-1" v-if="view === 1">
        <p>this is my 1st self-defined Vue component</p>
        {{ data }}
    </div>

    <div class="container-2" v-if="view === 2">
        <p>this is my 2nd self-defined Vue component</p>
        <input type="text" v-model="text" />
        <p>{{ text }}</p>
    </div>
</template>

<script setup>
    import { ref } from "@vue/reactivity"

    const data = 'fixed value'
    const text = ref("hello")

    const view = ref(1)

    const changeView = (index) => {
        view.value = index
    }
</script>

<style >

</style>