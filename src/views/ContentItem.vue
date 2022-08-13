<template>
    <div class="js-page">
        <ExampleInput></ExampleInput>
        <ExampleBinding></ExampleBinding>
        <ExampleList></ExampleList>
        <ExampleForm></ExampleForm>
        <ExampleObject></ExampleObject>
        <ExampleHover></ExampleHover>
    </div>
</template>

<script>
import ExampleHover from '@/components/ExampleHover.vue'
import ExampleInput from '@/components/Example-Input.vue'
import ExampleBinding from '@/components/Example-Binding.vue'
import ExampleList from '@/components/Example-List.vue'
import ExampleForm from '@/components/Example-Form.vue'
import ExampleObject from '@/components/Example-Object.vue'

export default {
    name: 'ContentItem',
    components: {
        ExampleInput,
        ExampleBinding,
        ExampleList,
        ExampleForm,
        ExampleObject,
        ExampleHover,
    }
}
</script>

<style scoped>
.js-page {
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-bottom: 3em;
}
</style>