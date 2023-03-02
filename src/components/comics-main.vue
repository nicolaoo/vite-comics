<script >
export default {
    data() {
        return {

        }
    }
}
</script>

<template>
    <main>
        <figure>
            <img class="bg-cartoon" src="/vue-dc-comics-1/img/jumbotron.jpg" alt="">
        </figure>
        <div class="comics-bg-black">
            <div class="container">
                <div>
                    <h2 class="title-comics">
                        --> content goes here
                    </h2>
                </div>
            </div>
        </div>
        <div class="comics-bg-blue">
            <div class="container">
                <div class="reidirector">
                    <div class="col">
                        <img src="vue-dc-comics-1/img/buy-comics-digital-comics.png" alt="">
                        <h4>digital comics</h4>
                    </div>
                    <div class="col">
                        <img src="vue-dc-comics-1/img/buy-comics-merchandise.png" alt="">
                        <h4>dc merchandise</h4>
                    </div>
                    <div class="col">
                        <img src="vue-dc-comics-1/img/buy-comics-shop-locator.png" alt="">
                        <h4>subscription</h4>
                    </div>
                    <div class="col">
                        <img src="vue-dc-comics-1/img/buy-comics-subscriptions.png" alt="">
                        <h4> coming shop locator</h4>
                    </div>
                    <div class="col">
                        <img src="vue-dc-comics-1/img/buy-dc-power-visa.svg" alt="">
                        <h4>dc power visa</h4>
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>

<style lang="scss" scoped>
.bg-cartoon {
    aspect-ratio: 18/4;
    object-fit: cover;
    object-position: top;
}

.comics-bg-black {
    background-color: black;
}

.comics-bg-blue {
    background-color: rgb(15, 124, 197);
    position: relative;
    z-index: 7;
}

.title-comics {
    color: white;
    padding: 30px 0;
}

.reidirector {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 30px 20px;
    color: white;

    .col {
        display: flex;
        gap: 10px;
        justify-content: center;
        align-items: center;

        img {
            width: 30px;

        }

        h4 {
            text-align: start;
            text-transform: uppercase;
            font-size: 10px;
        }
    }
}
</style>
