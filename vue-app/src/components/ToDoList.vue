<template>
    <div>
        <ul>
            {{todos}}
            <ToDoItem/>
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