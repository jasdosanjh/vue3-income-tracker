<template>
  <Header :totalIncome="state.totalIncome" />
</template>

<script>
import Header from '@/components/Header';
import { reactive, computed } from 'vue';

export default {
  components: {
    Header
  },

  setup() {
    const state = reactive({
      income: [],
      totalIncome: computed(() => state.income.reduce((total, { value }) => total + value, 0))
    })

    return {
     state
    }
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  background: #EEE;
}
</style>
