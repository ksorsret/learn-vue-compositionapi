<template>
  <h3>Method</h3>
  <button @click="handleFill">Click</button>
</template>

<script>
export default {
  setup() {
    const handleFill = () => {
      // Logic for filling the form
      console.log('Form filled successfully');
    }

    return {
      handleFill
    }
  }
}
</script>

<style>

</style>