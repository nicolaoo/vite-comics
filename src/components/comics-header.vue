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
                <div>

                    <a href="#">
                        <img class="logo" src="vue-dc-comics-1/img/favicon.ico" alt="">
                    </a>
                </div>
                <ul class="nav">
                    <li class="item-nav active">Lorem</li>
                    <li class="item-nav">Lorem</li>
                    <li class="item-nav">Lorem</li>
                    <li class="item-nav">Lorem</li>
                    <li class="item-nav">Lorem</li>
                    <li class="item-nav">Lorem</li>
                    <li class="item-nav">Lorem</li>
                    <li class="item-nav">Lorem</li>
                    <li class="item-nav">Lorem</li>
                    <li class="item-nav">Lorem</li>
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

.container {
    margin: 0 auto;
    max-width: 900px;

}

.nav {
    display: flex;

}

.logo {
    min-width: 40px;
}

* {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

.item-nav {
    padding: 10px;
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
    margin: auto;
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
    margin: auto;
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
