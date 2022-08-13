<template>
    <div class="object-wrap">
        <h1>simple component</h1>
        <ol>
            <TodoItem v-for="item in groceryList" v-bind:key="item"
            :todo="item"
            ></TodoItem>
        </ol>
    </div>
</template>

<script>
import TodoItem from '../TodoItem.vue'

export default {
    components: {
        TodoItem
    },
    data() {
        return {
            groceryList: [
                { id: 0, text: 'Vegetables'},
                { id: 1, text: 'Cheese'},
                { id: 2, text: 'other things'}
            ]
        }
    }
}
</script>

<style scoped>
.object-wrap {
    background: lightgray;
    margin-top: 20px;
}
</style>