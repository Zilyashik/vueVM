<template>
  <div>
    <h1>ToDo application</h1>
    <ToDoList
    :todos="todos"
    />
  </div>
</template>

<script>
import ToDoList from '@/components/ToDoList'
export default {
  name: 'App',
  data() {
    return {
      todos: [
        {id: 1, title: 'Купить дом', completed: false},
        {id: 2, title: 'Купить машину', completed: false},
        {id: 3, title: 'Купить банк', completed: false}
      ]
    }
  },
  components: {
    ToDoList
  }
}
</script>

<style>

</style>
