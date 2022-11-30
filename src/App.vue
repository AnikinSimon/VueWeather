<template>
  <div class="app">
    <InformerContainer/>
  </div>
</template>

<script>
import InformerContainer from './components/InformerContainer.vue'

export default {
  name: 'App',
  components: {
    InformerContainer
  }
}
</script>

<style>
  body {
    margin: 0;
    padding: 0;
  }

  .app {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100vh;
    background: rgb(244, 123, 186);
    background: linear-gradient(-25deg, rgba(244, 123, 186, 0.5) 20%, rgba(90, 95, 245, 0.5) 80%);
  }
</style>
