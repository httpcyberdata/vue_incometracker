<template>
  <div class="income-list">
    <IncomeItem v-for="data in state.sortedIncome" :key="data.id" :income="data" />
  </div>
</template>

<script>
import IncomeItem from './IncomeItem';
export default {
    props: {
        state: Object
    },
    components: {
        IncomeItem
    }
}
</script>

<style>
.income-list {
    margin-top: 30px;
    padding: 15px;
}
</style>