<template>
  <div id="app">
    <BudgetList :list="list"/>
  </div>
</template>

<script>

import BudgetList from "@/components/BudgetList";

export default {
  name: 'App',
  components: {
    BudgetList,
  },
  data: () => ({
    list: {
      1: {
        type: 'INCOME',
        value: 1000,
        comments: 'Some Comments Income',
        id: 1,
      },
      2: {
        type: 'OUTCOME',
        value: -100,
        comments: 'Some Comments Outcome',
        id: 2,
      },
    },
  }),
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
