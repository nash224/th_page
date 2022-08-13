<template>
    <div class="view-main">
        <div class="bg-fullpage">
            <div class="main-wrap">
                <img src="@/assets/forest-pic1.jpg" >
            </div>
        </div>
    </div>
</template>

<style scoped>
.view-main {
    margin-top: 0;

}
.bg-fullpage {
    width: 100vw;
    height: 600px;
    background-image: url("@/assets/content1-background.jpg");
}
.main-wrap {
    padding-top: 500px;
    margin: 0 10vw;
   
}
.main-wrap > img {
    width: 100vw;
    height: 60vh;
    object-fit: cover;
}

</style>