<template>
  <Header :totalIncome="state.totalIncome"/>
  <Form />
</template>

<script>
import { reactive, computed } from 'vue';
import Header from './components/Header';
import Form from './components/Form.vue';
export default {
  setup() {
    const state = reactive({
      income: [],
      totalIncome: computed(() => {
        let temp = 0;
        if(state.income.length > 0) {
          for(let i = 0; i < state.income.length; i++) {
            temp += state.income[i].value;
          }
        }
        return temp;
      })
    })
    return {
      state
    }
  },
  name: 'App',
  components: {
    Header,
    Form
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
