<template>
  <div>
    <ul>
      <ToDoItem
      v-for="todo in todos"
      :key="todo"
      :todo="todo"
      />
    </ul>
  </div>
</template>

<script>
import ToDoItem from "@/components/ToDoItem";
export default {
  name: "ToDoList",
  props: ['todos'],
  components: {
    ToDoItem
  }
}
</script>

<style scoped>
  ul {
    list-style: none;
    margin: 0;
    padding: 0;
  }
</style>