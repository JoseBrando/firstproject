<template>
    <p v-bind:style="{
        backgroundColor : 'red',
        color: '#fff'
    }">El mensaje se ha enviado satisfactoriamente.</p>
</template>

<script lang="ts" setup>
    let hasError:Boolean = true;
</script>

<style scoped>

</style>