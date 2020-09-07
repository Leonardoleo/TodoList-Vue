<template>
<div>
    <input type="text" class="todo-input" placeholder="What needs to be done">
    Todo List goes here
</div>
</template>

<script>
export default {
  name: 'todo-list',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>


<style>
  .todo-input {
      width: 100%;
      padding: 10px 10px;
      font-size: 18px;
      margin-bottom: 10px;
  }

    input:focus {
        outline: 0;
    }

</style>
