<template>
  <h3>Computed</h3>
  <p>{{ computedValue }}</p>
  <input type="text" v-model="age">
</template>

<script>
import { computed, ref } from 'vue';
export default {
setup() {
  const age = ref(10);
  const computedValue = computed(() => {
    // Perform complex calculations or transformations here
    return age.value + 10;
  });

  return {
    computedValue,
    age,
  };
}
}
</script>

<style>

</style>