<template>
    <div class="js-page">
        <CssHover></CssHover>
        <logincom></logincom>
        <ExampleInput></ExampleInput>
        <ExampleBinding></ExampleBinding>
        <ExampleList></ExampleList>
        <ExampleForm></ExampleForm>
        <ExampleHover></ExampleHover>
    </div>
</template>

<script>
import ExampleHover from '@/components/Example/ExampleHover.vue'
import ExampleInput from '@/components/Example/Example-Input.vue'
import ExampleBinding from '@/components/Example/Example-Binding.vue'
import ExampleList from '@/components/Example/Example-List.vue'
import ExampleForm from '@/components/Example/Example-Form.vue'
import CssHover from '@/components/Example/CssHover.vue'
import logincom from '@/components/Example/LoginCom.vue'

export default {
    name: 'ContentItem',
    components: {
        ExampleInput,
        ExampleBinding,
        ExampleList,
        ExampleForm,
        ExampleHover,
        CssHover,
        logincom,
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