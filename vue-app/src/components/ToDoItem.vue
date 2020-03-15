<template>
    <div class="itemContainer">
        <div class="headerBlock">
            <input type="checkbox">
            <strong>{{todo.id}}</strong>
            {{todo.title}}
        </div>
        <img :src="todo.imgSrc" class="pic" />
    </div>
</template>

<script>
export default {
    props: {
        todo:{
            type: Object,
            required: true
        }
    }
}
</script>