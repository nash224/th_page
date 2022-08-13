<template>
    <div class="Ch">
        <a href="/"><span>Hover me</span></a>
    </div>
</template>


<style scoped>
.Ch {
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 0;
    margin-bottom: 30px;
}
.Ch a {
    position: relative;
    width: 170px;
    height: 50px;
    text-align: center;
    background: linear-gradient(140deg, #ff6060, #4d4df7, #64ff64, #ff63ff);
    border-radius: 10px;
}
.Ch a > span {
    height: 82%;
    width: 95%;
    font-family: Moderat;
    color: #f2f2f2;
    font-size: 1.4em;
    font-weight: 400;
    letter-spacing: 2px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    background: #111;
    border-radius: 8px;
    line-height: 36px;
}
.Ch a:hover {
    animation: Chs 0.6s linear infinite;
}
@keyframes Chs {
    to {
        filter: hue-rotate(-360deg);
    }
}
</style>