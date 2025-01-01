<template>
  <div
    class="card border-primary"
  >
    <div class="card-body">
      <h4 class="card-title">Title: {{ username }}</h4>
      <p class="card-text">Text</p>
    </div>
  </div>
  
</template>

<script>
import { reactive, ref } from 'vue'
export default {
  setup() {
    const username = ref('initvalue');
    const form = reactive({
      email: 'email@example.com',
      password: 'password'
    })
    setTimeout(() => {
      username.value = '111';
    }, 2000);

    return {
      username,
      form
    }
  }
}
</script>

<style>

</style>