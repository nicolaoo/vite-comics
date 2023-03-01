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
                        <li>lorem</li>
                        <li>lorem</li>
                        <li>lorem</li>
                        <li>lorem</li>
                        <li>lorem</li>
                        <li>lorem</li>
                        <li>lorem</li>

                        <h4 class="title-link-site">shop</h4>
                        <li>lorem</li>
                        <li>lorem</li>
                    </div>
                    <div class="links dc">
                        <h4 class="title-link-site">dc</h4>
                        <li>lorem</li>
                        <li>lorem</li>
                        <li>lorem</li>
                        <li>lorem</li>
                        <li>lorem</li>
                        <li>lorem</li>
                        <li>lorem</li>
                        <li>lorem</li>
                    </div>
                    <div class="links sites">
                        <h4 class="title-link-site">sites</h4>
                        <li>lorem</li>
                        <li>lorem</li>
                        <li>lorem</li>
                        <li>lorem</li>
                        <li>lorem</li>
                    </div>
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

<style >
.container {
    margin: 0 auto;
    max-width: 900px;

}

* {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}


ul,
li {
    list-style-type: none;

}

img {
    max-width: 100%;
}

/* REGOLE FOOTER  */

.foot-size {
    background-image: url("vue-dc-comics-1/img/footer-bg.jpg");
    padding: 20px 0;
}

.foot-social {
    background-color: rgb(63, 63, 63);
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
    color: white;
    font-size: 10px;
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
}

.btn-sign {
    border: 2px solid rgb(15, 124, 197);
    font-size: 12px;
    text-transform: uppercase;
    padding: 10px;
    background-color: rgb(63, 63, 63);
    color: white;
    font-weight: 600;
}

.icon-social h4 {
    font-size: 12px;
    text-transform: uppercase;
    padding: 10px;
    background-color: rgb(63, 63, 63);
    color: rgb(15, 124, 197);
    font-weight: 700;
}

.social {
    gap: 20px;
}
</style>
