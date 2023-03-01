<script >

export default {
    data() {
        return {

        }
    }
}

</script>

<template>
    <div class="header">
        <div class="container">
            <div class="head-section">
                <a href="#">
                    <img class="logo" src="vue-dc-comics-1/img/favicon.ico" alt="">
                </a>
                <ul class="nav">
                    <li class="item-nav active">characters</li>
                    <li class="item-nav">comics</li>
                    <li class="item-nav">movies</li>
                    <li class="item-nav">tv</li>
                    <li class="item-nav">games</li>
                    <li class="item-nav">collectibles</li>
                    <li class="item-nav">videos</li>
                    <li class="item-nav">fans</li>
                    <li class="item-nav">news</li>
                    <li class="item-nav">shop</li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style>
.header {
    position: relative;
}

.head-section {
    display: flex;
    justify-content: space-between;
    padding: 20px 0;
    align-items: center;

}

.nav {
    display: flex;

}

* {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

.item-nav {
    padding: 0 10px;
    color: rgb(63, 63, 63);
    text-transform: uppercase;
    font-size: 12px;
    font-weight: 600;
}

.item-nav:hover {
    color: rgb(15, 124, 197);
}

.item-nav:hover::after {
    opacity: 0.9;
    color: rgb(15, 124, 197);
    content: '';
    display: block;
    width: 40px;
    height: 5px;
    background-color: rgb(15, 124, 197);
    position: absolute;
    bottom: 0;
}

.item-nav.active {
    color: rgb(15, 124, 197);
}

.active::after {
    content: '';
    display: block;
    width: 40px;
    height: 5px;
    color: rgb(15, 124, 197);
    background-color: rgb(15, 124, 197);
    position: absolute;
    bottom: 0;

}

ul {
    list-style-type: none;
}

img {
    max-width: 100%;
}
</style>
