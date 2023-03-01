<script >

export default {
    data() {
        return {

        }
    }
}

</script>

<template>
    <div class="container">
        <div class="header">
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
</template>

<style>
.header {
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
    opacity: 0.9;
    color: rgb(15, 124, 197);
}

.item-nav.active {
    color: rgb(15, 124, 197);
}


ul {
    list-style-type: none;
}

img {
    max-width: 100%;
}
</style>
