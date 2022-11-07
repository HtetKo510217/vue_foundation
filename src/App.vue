<template>
  <div class="container" @click.self="hideModal">
    <ModalBox v-if="showModal" theme="success">
      <h1>Success Modal Box</h1>
      <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit</p>
    </ModalBox>
    <ModalBox v-if="deleteModal" theme="delete">
      <h1>Dlete modal</h1>
      <p>Are you sure you want to delete ?</p>
    </ModalBox>
  </div>
  <button @click="showModal = true">Show Modal</button>
  <button @click="deleteModal=true">Delete Modal</button>
</template>

<script>
import ModalBox from './components/ModalBox.vue'
export default {
  name: 'App',
  components: {
    ModalBox,
  },
  data() {
    return {
      showModal : false,
      deleteModal : false,
    }
  },
  methods: {
    hideModal () {
      this.showModal = false,
      this.deleteModal = false
    }
  }
}
</script>

<style>
#app {
  text-align: center;
}
button {
  margin-left: 10px;
}
</style>
