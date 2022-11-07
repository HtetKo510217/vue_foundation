<template>
  <div class="modalBox" :class="theme">
    <slot>Modal box</slot>
  </div>
</template>

<script>
export default {
    props: ['theme']
}
</script>

<style scoped>
 .modalBox {
    width: 400px;
    height: 300px;
    box-sizing: border-box;
    margin: 10px auto;
    color: #fff;
    padding: 10px;
}
.success {
    background: darkgreen;

}
.delete {
    background: darkred;
}

</style>