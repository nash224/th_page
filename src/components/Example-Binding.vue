<template>
    <div class="bind-wrap">
        <div class="bind-box A">
            <h1>click event</h1>
            <p :class="{ red: isRed }" @click="toggleRed">
                Change style's exist, if you click this 
            </p>
            <p :style="{ color }" @click="toggleColor">
                Change only font-color
            </p>
        </div>
        
        <!-- <div class="bind-box B">
            <h1>click evnet2</h1>
            <p :class="{ green: IsSize }" @click="toggleSize">
                Change this style's exist, click me!
            </p>
        </div> -->
    </div>
</template>

<script>

export default {
    data() {
        return {
            msg: 'What is this color',
            isRed: true,
            isColor: true,
            color: 'green',
        }
    },
    methods: {
        toggleRed() {
            this.isRed = !this.isRed
        },
        toggleColor() {
            this.color = this.color === 'green'? 'blue':'green'
        },
        toggleSize() {
            this.IsSize = !this.isSize
        },

    }
}
</script>

<style scoped>
.red {
    color: red;
    background: lightgrey;
}
.green {
    background-color: blue;
}

</style>