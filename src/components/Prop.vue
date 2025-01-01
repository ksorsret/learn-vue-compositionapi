<template>
  <h3>Props</h3>
</template>

<script>
import { toRefs } from 'vue';
export default {
  props: {
    abc: String
  },
  setup(props) {
    const {abc} = toRefs(props);
    console.log('>>>',abc);
  }
}
</script>

<style>

</style>