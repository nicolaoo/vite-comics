<script >
export default {
    data() {
        return {
            heroCard: [
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book"
                },
                {
                    "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book"
                },
                {
                    "thumb": "https://picsum.photos/200/300",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel"
                }
            ],
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
                <div class="grid">
                    <div v-for="(el, i) in heroCard" :key="i" class="card">
                        <figure>
                            <img src="https://picsum.photos/200/300" alt="">
                        </figure>
                        <p>
                            {{ el.series }}
                        </p>
                    </div>
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

.card {
    p {
        color: white;
        text-transform: uppercase;
        font-size: 10px;
    }
}

.grid {
    display: grid;
    grid-template-columns: repeat(6, 1fr);
    gap: 20px;
    padding: 20px 0;
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
