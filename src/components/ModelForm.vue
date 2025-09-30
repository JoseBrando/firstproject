<template>
    <form>
        <input type="text" v-model="inputText">
        <input type="checkbox" v-model="agree"> Acepto los términos y condiciones
        <select v-model="countrySelect">
            <option v-for="country in countries" v-bind:value="country.code">{{ country.name }}</option>
        </select>
    </form>

    <h3>{{ inputText }}</h3>
</template>

<script lang="ts" setup>
    import type { ICountry } from '@/interfaces/ICountry'
    import type { Ref } from 'vue'
    import {ref} from 'vue'

    let inputText:Ref<String> = ref('');
    let agree:Ref<Boolean> = ref(true)
    let countries:Ref<Array<ICountry>> = ref([
        {
            code: 'es',
            name: 'Spain'
        },
        {
            code: 'en',
            name: 'UK'
        },
        {
            code: 'fr',
            name: 'France'
        },
        {
            code: 'it',
            name: 'Italy'
        },
        {
            code: 'pt',
            name: 'Portugal'
        }
    ])
    let countrySelect:Ref<String> = ref('es')
</script>

<style scoped>

</style>