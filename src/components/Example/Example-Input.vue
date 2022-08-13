<template>
    <h1>{{ user_input }}</h1>
    <div class="input-wrap">
        <div class="input-box A">
            <button @click="reverseMessage">reverse</button>
            <button @click="user_input += '!'">append</button>
            <a href="/" @click.prevent="notify">alert!</a>
        </div>

        <div class="input-box B">
            <h1>{{ my_practices1 }}</h1>
            <button @click="reverseMsg">reverse</button>
            <button @click="my_practices1 += '?'">append</button>
        </div>
    </div>
</template>


<script>
export default {
    data() {
        return {
            user_input: 'user input!',
            my_practices1: 'Is this vue?'
        }
    },
    methods: {
        reverseMessage() {
            this.user_input = this.user_input.split('').reverse().join('')
        },
        reverseMsg() {
            this.my_practices1 = this.my_practices1.split('').reverse().join('')
        },
        notify() {
            alert('navigation was prevented!!!')
        }
    }
}
</script>

<style scoped>
.input-wrap {
    display: flex;
    flex-direction: column;
    flex-basis: auto;
    margin-top: 5px;
}
/* h1 {
    padding-top: 1em;
} */
button, a {
    /* display: flex;
    flex-direction: column;
    justify-content: center; */
    padding: 2px;
    margin-right: 10px;
}
.input-box {
    padding-bottom: 2em;
}
.B {
    margin-bottom: 1em;
}
</style>