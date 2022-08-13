<template>
    <div class="hover-text-wrap">
        <h1>Is this work?</h1>
    </div>
</template>

<style scoped>
h1 {
    position: relative;
    margin-top: 30px;
}
h1::before {
    transform: scaleX(0);
    transform-origin: right;
}
h1:hover::before {
    transform: scaleX(1);
    transform-origin: left;
}
h1::before {
    content: " ";
    inset: 0;
    position: absolute;
    top: 0; right: 0; bottom: 0; left: 0;
    background: hsl(120, 60%, 70%);
    z-index: -1;
    transition: transform 0.3s;
    
}
</style>