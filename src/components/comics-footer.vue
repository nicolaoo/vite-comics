<script >
export default {
    data() {
        return {

        }
    }
}


</script>

<template>
    <footer>
        <div class="foot-size">
            <div class="container">
                <div class="link-site">
                    <div class="links comics-shop">
                        <h4 class="title-link-site">dc comics</h4>
                        <li>characters</li>
                        <li>comics</li>
                        <li>movies</li>
                        <li>tv</li>
                        <li>games</li>
                        <li>collectibles</li>
                        <li>videos</li>

                        <h4 class="title-link-site">shop</h4>
                        <li>fans</li>
                        <li>news</li>
                    </div>
                    <div class="links dc">
                        <h4 class="title-link-site">dc</h4>
                        <li>shop</li>
                        <li>news</li>
                        <li>fans</li>
                        <li>videos</li>
                        <li>collectibles</li>
                        <li>games</li>
                        <li>tv</li>
                        <li>movies</li>
                    </div>
                    <div class="links sites">
                        <h4 class="title-link-site">sites</h4>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Poer Visa</li>
                    </div>
                    <figure>
                        <img class="logo-dc-big" src="vue-dc-comics-1/img/dc-logo-bg.png" alt="">
                    </figure>
                </div>
            </div>
        </div>
        <div class="foot-social">
            <div class="container">
                <div class="profile-social">
                    <div>
                        <button class="btn-sign">
                            sign-up now!
                        </button>
                    </div>
                    <div class="icon-social">
                        <h4>follow us</h4>
                        <ul class="social">
                            <li><img src="vue-dc-comics-1/img/footer-facebook.png" alt=""></li>
                            <li><img src="vue-dc-comics-1/img/footer-twitter.png" alt=""></li>
                            <li><img src="vue-dc-comics-1/img/footer-youtube.png" alt=""></li>
                            <li><img src="vue-dc-comics-1/img/footer-pinterest.png" alt=""></li>
                            <li><img src="vue-dc-comics-1/img/footer-periscope.png" alt=""></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables.scss' as *;

.foot-size,
.foot-social {
    z-index: 5;
    position: relative;
}

.logo-dc-big {
    position: absolute;
    right: 100px;
    z-index: 0;
    width: 400px;
    bottom: -45px;
}

.foot-size {
    background-image: url("vue-dc-comics-1/img/footer-bg.jpg");
    padding: 20px 0;
}

.foot-social {
    background-color: $grey-footer;
}

.link-site {
    display: flex;
    gap: 30px;

}

.title-link-site {
    color: white;
    text-transform: uppercase;
    font-size: 12px;
    padding: 10px 0;

}

.links li {
    color: #ffffff;
    opacity: 0.5;
    font-size: 12px;
    padding: 2px 0;
}

.profile-social,
.icon-social,
.social {
    display: flex;
}

.profile-social {
    justify-content: space-between;
    align-items: center;
    padding: 20px 0;
}

.icon-social {
    gap: 20px;
    align-items: center;

    h4 {
        font-size: 15px;
        text-transform: uppercase;
        padding: 10px;
        background-color: $grey-footer;
        color: $azure;
        font-weight: 700;
    }

    .social {
        gap: 20px;
    }
}

.btn-sign {
    border: 2px solid $azure;
    font-size: 12px;
    text-transform: uppercase;
    padding: 10px;
    background-color: $grey-footer;
    color: white;
    font-weight: 600;
}
</style>
