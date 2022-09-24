<template>
  <button class="btn" :class="btnclass">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: 'ProjectFormButton',
  props: {
    text: String,
    btnclass: String
  }
}
</script>

<style scoped>
  .btn {
  padding: 10px 20px;
  border-radius: 5px;
  cursor: pointer;
  }

  .add {
    border: 1px solid #99dd99;
    background-color: #aaffaa;
    font-weight: bold;
  }

  .cancel {
    border: 1px solid #eeadad;
    background-color: #ffbebe;
    font-weight: bold;
  }
</style>
