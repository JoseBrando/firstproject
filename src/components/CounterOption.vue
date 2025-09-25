<template>
    <h3>{{ counter }}</h3>
    <button @click="addCounter">Incrementar</button>
</template>

<script lang="ts">
    import { defineComponent } from 'vue'; // permite definir componentes
    export default defineComponent({
        name: 'CounterOption',
        components: {},
        data() {
            let counter = 100;
            return { counter, incremento: 1 }
        },
        methods: {
            addCounter() {
                this.counter += this.incremento
            }
        }
    })
</script>
