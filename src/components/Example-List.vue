<template>
    <div class="list-wrap">
        <div class="manage-list">
            <h1>Add/Rm list</h1>
            <button @click="show = !show">Toggle List</button>
            <button @click="list.push(list.length + 1)">Push</button>
            <button @click="list.pop()">Pop</button>
            <button @click="list.reverse()">Reverse list</button>
            <ul v-if="show && list.length">
                <li v-for="item of list" v-bind:key="item">{{ item }}</li>
            </ul>
            <p v-else-if="list.length">List is not empty, but hidden.</p>
            <p v-else>List is empty.</p>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            show: true,
            list: [1, 2, 3]
        }
    }
    
}
</script>

<style scoped>
h1 {
    /* margin-top: 20px; */
    margin-bottom: 20px;
}
button {
    margin-right: 10px;
    margin-bottom: 20px;
}
ul {
    list-style: none;
}
.list-wrap {
    margin-top: 20px;
    background: lightgray;
}
</style>