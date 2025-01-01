<template>
  <h3>Watch {{ age }}</h3>
  <button @click="handleIn">Incrêmt</button>
</template>

<script>
import { ref, watch } from 'vue'
export default {
  setup() {
    const age = ref(10);
    function handleIn() {
      age.value++;
    }

    watch(age, function(newValue, oldValue) {
      console.log(newValue, oldValue);
    });

    return {
      age,
      handleIn
    }
  }
}
</script>

<style>

</style>