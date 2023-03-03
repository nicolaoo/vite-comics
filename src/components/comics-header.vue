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
                    <img class="logo" src="vue-dc-comics-1/img/dc-logo.png" alt="">
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

<style lang="scss" scoped>
@use '../style/partials/variables.scss' as *;

.header {
    position: relative;
}

.logo {
    max-width: 60px;
}

.head-section {
    display: flex;
    justify-content: space-between;
    padding: 10px 0;
    align-items: center;

}

.nav {
    display: flex;

    .active {
        color: $azure;

        &::after {
            content: '';
            display: block;
            width: 40px;
            height: 5px;
            color: $azure;
            background-color: $azure;
            position: absolute;
            bottom: 0;

        }


    }

}

.item-nav {
    padding: 0 10px;
    color: $grey-footer;
    text-transform: uppercase;
    font-size: 12px;
    font-weight: 600;

    &:hover {
        color: $azure;

        &::after {
            opacity: 0.9;
            color: $azure;
            content: '';
            display: block;
            width: 40px;
            height: 5px;
            background-color: $azure;
            position: absolute;
            bottom: 0;
        }
    }
}
</style>
