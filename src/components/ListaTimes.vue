<template>
  <h1>Times</h1>

  <BotomTime v-for="time in times" v-bind:key="time" :nomeTime="time" />
</template>

<script>
import BotomTime from './BotomTime.vue'

export default {
  name: 'ListaTimes', //nome do componente
  components: { BotomTime },
  props: {
    times: Array,
  },
}
</script>

<style></style>
