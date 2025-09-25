<template>
  <h1>Curso Profesional</h1>
  <CounterComposition/>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import CounterComposition from './components/CounterComposition.vue';

export default defineComponent({
  name: 'App',
  components: {
    CounterComposition
  }
})
</script>

<style scoped></style>
