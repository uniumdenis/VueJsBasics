<template>
    <div>
        <ul>
            <ToDoItem 
                v-for="todo of todos" 
                v-bind:key="todo.id"
                v-bind:todo="todo">
            </ToDoItem>
        </ul>
    </div>
</template>

<script>
import ToDoItem from '@/components/ToDoItem'
export default {
    props: ['todos'],
    components:{
        ToDoItem
    }
}
</script>