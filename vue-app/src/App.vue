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
        {
          id: 1, 
          title: 'Установить VS Code', 
          completed: false,
          imgSrc: "https://svirtus.cdnvideo.ru/x3CupDa2riY9sVL29KXaYABq4Ys=/0x0:1236x654/1240x525/filters:quality(100)/https://hb.bizmrg.com/cybersportru-media/44/44fe2892c08549bad08f5cf2a17d7ca1.jpg?m=4af28815a3587b23c9ba45aece8fd193"
        },
        {
          id: 2, 
          title: 'Сделать fork https://github.com/grishinrv/VueJsBasics', 
          completed: false,
          imgSrc: "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcRt50q9N3icik2BfkY50hmXF25-u0OurM2zLEXL81lN15vGpskI"
        },
        {
          id: 3, 
          title: 'Разработать просто приложение-список', 
          completed: false,
          imgSrc: "https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcQesmcBXMT9k1JFVpWeKmc2MW45YhclQMBPMJqxVeY40xDuU4Nd"
        }
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
