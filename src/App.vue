<template>
  <Header />
</template>

<script>
import Header from './components/Header'
import { reactive, computed } from 'vue';
export default {
  setup() {
    const state = reactive({
      income: [],
    })
  },
  name: 'App',
  components: {
    Header
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Fire Code', sans-serif;
}

body {
  background: #EEE;
}
</style>
