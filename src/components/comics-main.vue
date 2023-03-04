<script >
import vignette from "./cicolo-for-vignette.vue"
export default {
    data() {
        return {
            heroCard: [
                {
                    "thumb": "https://www.freekomix.it/wp-content/uploads/2023/01/SUPERMAN-ACTION-COMICS-2.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://mlpnk72yciwc.i.optimole.com/cqhiHLc.IIZS~2ef73/w:auto/h:auto/q:75/https://bleedingcool.com/wp-content/uploads/2021/05/AQM_80THANN_Cv11_60a2d6ea2f7545.69069474-1.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://i0.wp.com/www.lideachetimanca.com/wp-content/uploads/2020/07/5050574343640.jpg?resize=300%2C460&ssl=1",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/m/1/m1batm001_0_yrafgywzsh7c1i8l.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://upload.wikimedia.org/wikipedia/it/8/8d/Batman_beyond_1-195x300.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.tvtropes.org/pmwiki/pub/images/superman_5.png",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://content1.jdmagicbox.com/comp/jd_social/news/2018jul06/image-1881-d78cee.jpg?fit=around|210:308&crop=210:308;*,*",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://static.posters.cz/image/750webp/73582.webp",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://i0.wp.com/www.lideachetimanca.com/wp-content/uploads/2020/07/5050574339056.jpg?resize=300%2C460&ssl=1",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://i0.wp.com/www.lideachetimanca.com/wp-content/uploads/2020/07/5050574341486.jpg?fit=350%2C528&ssl=1",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/m/1/m1anni001isbn_0.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ],
        }
    },
    components: {
        vignette
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
                <button class="btn-first-vignet">
                    load more
                </button>
                <div class="grid">
                    <vignette v-for="(el, i) in heroCard" :key="i" :src="el.thumb" :text="el.series" />
                </div>
                <button class="btn-second-vignet">
                    load more
                </button>
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
@use '../style/partials/variables.scss' as *;

.container {
    text-align: center;
}

.bg-cartoon {
    aspect-ratio: 18/4;
    object-fit: cover;
    object-position: top;
}

.comics-bg-black {
    background-color: black;
}

.comics-bg-blue {
    background-color: $azure;
    position: relative;
    z-index: 7;
}

.grid {
    display: grid;
    grid-template-columns: repeat(6, 1fr);
    gap: 20px;
    padding: 30px;
}

.reidirector {
    display: flex;
    justify-content: space-between;
    align-items: center;
    color: white;
    padding: 20px;

    .col:hover {
        background-color: rgb(255, 255, 255, 0.2);

        border-radius: 10px;
    }

    .col {
        display: flex;
        gap: 10px;
        justify-content: center;
        align-items: center;
        padding: 10px;

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

.btn-second-vignet {
    margin-bottom: 15px;
    padding: 7px 45px;
    background-color: $azure;
    color: white;
    text-transform: uppercase;
    font-size: 13px;
    font-weight: 600;
}

.btn-first-vignet {
    padding: 7px 45px;
    background-color: rgb(2, 130, 249);
    color: white;
    text-transform: uppercase;
    font-size: 13px;
    font-weight: 600;
    position: absolute;
    top: 60%;
    left: 16%;
}
</style>
