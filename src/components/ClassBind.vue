<template>
    <p v-bind:style="{
        backgroundColor : 'black',
        color: blanco
    }">El mensaje se ha enviado satisfactoriamente.</p>

    <button v-on:click="handleClick()">Cambiar color</button>
</template>

<script lang="ts" setup>
    import {ref} from 'vue';

    let blanco = ref('#fff');
    const handleClick = () => blanco.value = '#ff0000'
</script>

<style scoped>

</style>