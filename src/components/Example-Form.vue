<template>
    <div class="bind-form-wrap">
        <h1>Bind Form</h1>
        <h2>Text Input</h2>
        <input v-model="text"><br/>{{ text }}

        <h2>Check box</h2>
        <input type="checkbox" id="ckeckbox" v-model="checked">
        <label for="checkbox">Checked {{ checked }}</label>

        <h2>Multi checkbox</h2>
        <input type="checkbox" id="roro" value="Roro" v-model="CheckedName">
        <label for="roro">Roro</label>
        <input type="checkbox" id="lala" value="Lala" v-model="CheckedName">
        <label for="lala">Lala</label>
        <input type="checkbox" id="coco" value="Coco" v-model="CheckedName">
        <label for="coco">Coco</label>
        <p>Chedked names: <pre>{{ CheckedName }}</pre></p>

        <h2>Radio</h2>
        <input type="radio" id="one" value="One" v-model="picked">
        <label for="one">One</label>
        <br>
        <input type="radio" id="two" value="Two" v-model="picked">
        <label for="two">Two</label>
        <br>
        <input type="radio" id="three" value="Three" v-model="picked">
        <label for="three">Three</label>
        <br>
        <span>Picked: {{ picked }}</span>

        <h2>Select</h2>
        <select v-model="selected">
            <option disabled value="">Please select one</option>
            <option>A</option>
            <option>B</option>
            <option>C</option>
        </select>
        <br>
        <span>Selected: {{ selected }}</span>

        <h2>Multi Select</h2>
        <select v-model="multiSelected" multiple style="width: 100px;">
            <option>A</option>
            <option>B</option>
            <option>C</option>
        </select>
        <br>
        <span>Selected: {{ multiSelected }}</span>
        
    </div>
</template>

<script>
export default {
    data() {
        return {
            text: "Input text",
            checked: true,
            CheckedName: ['Roro'],
            picked: 'One',
            selected: 'A',
            multiSelected: 'A'
        }
    }
}
</script>

<style scoped>
.bind-form-wrap {
    background: lightgray;
    margin-top: 20px;
}
</style>