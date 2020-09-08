<template>
<div>
    <input type="text" class="todo-input" placeholder="What needs to be done" v-model="newTodo" @keyup.enter="addTodo">
    <div v-for="todo in todos" :key="todo.id" class="todo-item">
    {{ todo.title }}
    </div>
</div>
</template>

<script>
export default {
  name: 'todo-list',
  // data
  data () {
    return {
      newTodo: '',
      todos:[
       {
          'id': 1,
          'title': 'Finish Vue Screencast',
          'completed': false,
       },
           {
          'id': 2,
          'title': 'Take over the world',
          'completed': false,
       },
      ]
    }
  },
  // methods
  methods: {
     addTodo() {
       alert('adding')
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
