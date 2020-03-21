<template>
    <div class="itemContainer">
        <div class="headerBlock">
            <button v-on:click="printHello(todo.id)">Нажми</button>
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
    },
    methods: {
        printHello (componentName){
            alert("Привет от "+componentName);
        }
    }
}
</script>