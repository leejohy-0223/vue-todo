<template>
  <div class="clearAllContainer">
<!--    <span class="clearAllBtn" @click="clearTodo">ClearAll</span>-->
    <button class="btn btn-danger" @click="clearTodo">ClearAll</button>
<!--    <button type="button" class="btn btn-danger">Danger</button>-->
  </div>
</template>

<script>
export default {
  name: "TodoFooter",
  methods: {
    clearTodo() {
      this.$emit('removeAll');
    }
  }
}
</script>

<style scoped>
  .clearAllContainer {
    width: 8.5rem;
    height: 50px;
    line-height: 50px;
    /*background-color: white;*/
    border-radius: 5px;
    margin: 0 auto;
  }
  .clearAllBtn {
    color: #e20303;
    display: block;
  }
</style>
