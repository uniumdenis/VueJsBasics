<template>
  <div id="app">
    <h1>Vue js app</h1> 
    <ToDoList
      v-bind:todos="todos"
    />
  </div>
</template>

<script>
import ToDoList from '@/components/ToDoList'
export default {
  name: 'app',
  data (){
    return {
      todos: [
        {id: 1, title: 'Установить VS Code', completed: false},
        {id: 2, title: 'Сделать fork https://github.com/grishinrv/VueJsBasics', completed: false},
        {id: 3, title: 'Разработать просто приложение-список', completed: false}
      ]
    }
  },
  components: {
    ToDoList
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
