<template>
    <div id="header" class="header">
        <div class="header-wrap">
            <div class="header-logo"></div>
            
            <div class="header-menu-inner">
                <div class="main-menu">
                    <ul>
                        <li><a href=""></a></li>

                    </ul>
                </div>
            </div>

            <div class="search-menu"></div>
        </div>
    </div>
</template>




<style scoped>
.header {
    overflow: hidden;
}
.header-wrap {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    width: 100vw;
    height: 70px;
    align-items: center;
    background: lightseagreen;

}
.header-logo {
    display: flex;
    align-items: center;
    width: 50px;
    margin-left: 30px;
    height: 50px;
    padding: 5px;
    background: lightgray;
    
}
.header-menu-inner {
    display: flex;
    align-items: center;
    width: 300px;
    height: 60px;
    background: lightcoral;
}
.search-menu {
    display: flex;
    align-items: center;
    width: 200px;
    height: 50px;
    margin-right: 70px;
    background: lightsalmon;
}
</style>