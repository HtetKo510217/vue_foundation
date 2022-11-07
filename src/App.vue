<template>
  <div>
    <ModalBox />
  </div>
</template>

<script>
import ModalBox from './components/ModalBox.vue'
export default {
  name: 'App',
  components: {
    ModalBox,
  }
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
