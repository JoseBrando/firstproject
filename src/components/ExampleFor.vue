<template>
    <ul>
        <li v-for="country in countries" :key="country.code as string">{{ country.name }}</li>
    </ul>
</template>

<script lang="ts" setup>
    import type {Ref} from 'vue';
    import {ref} from 'vue';
    import type {ICountry} from '../interfaces/ICountry'

    // let countries:Ref<Array<String>> = ref([
    //     'Spain', 'France', 'UK', 'Italy', 'Portugal'
    // ])

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
</script>

<style scoped>

</style>