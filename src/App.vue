<template>
  <div id="app">
  <p v-for="(value, key, index) in jokes" :key="value">
    {{ index }}. {{ key }}: {{ value }}
  </p>
</div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  data() {
    return {
      jokes: {
        question: 'What did one baby prototype say to the other?',
        answer: `I'll race you to class!`,
        response: 'groan'
      }
    }
  }
}
</script>
