<script>

export default {
    name: "AppFooter",
    props: {
        links: Object,
    },
    data() {
        return {

        }
    }
}
</script>

<template>
    <div class="container-fluid bg_container">
        <div class="container">
            <div class="row">
                <div class="col-2 py-5">
                    <div class="list-group">
                        <span class="text-white fw-bold pb-3">DC COMICS</span>
                        <div v-for="(link, c) in links" class="text-start">
                            <a href="" class="list-group-item border-0 text-start p-0" v-if="link.status == true">{{
                                link.link }}</a>
                        </div>
                        <span class="text-white fw-bold py-3">SHOP</span>
                        <div>
                            <a href="" class="list-group-item border-0 text-start p-0">Shop Dc</a>
                            <a href="" class="list-group-item border-0 text-start p-0">Shop Dc Collectibles</a>
                        </div>
                    </div>
                </div>
                <div class="col-2 py-5">
                    <div class="list-group">
                        <span class="text-white fw-bold pb-3">DC</span>
                        <div>
                            <a href="" class="list-group-item border-0 text-start p-0">Terms Of Use</a>
                            <a href="" class="list-group-item border-0 text-start p-0">Privacy policy(New)</a>
                            <a href="" class="list-group-item border-0 text-start p-0">Ad Choices</a>
                            <a href="" class="list-group-item border-0 text-start p-0">Advertising</a>
                            <a href="" class="list-group-item border-0 text-start p-0">jobs</a>
                            <a href="" class="list-group-item border-0 text-start p-0">Subscriptions</a>
                            <a href="" class="list-group-item border-0 text-start p-0">Talent Workshops</a>
                            <a href="" class="list-group-item border-0 text-start p-0">CPSC Certificates</a>
                            <a href="" class="list-group-item border-0 text-start p-0">Ratings</a>
                            <a href="" class="list-group-item border-0 text-start p-0">Shop Help</a>
                            <a href="" class="list-group-item border-0 text-start p-0">Contact Us</a>
                        </div>
                    </div>
                </div>
                <div class="col-2 py-5">
                    <div class="list-group">
                        <span class="text-white fw-bold pb-3">SITES</span>
                        <div>
                            <a href="" class="list-group-item border-0 text-start p-0">DC</a>
                            <a href="" class="list-group-item border-0 text-start p-0">MAD Magazine</a>
                            <a href="" class="list-group-item border-0 text-start p-0">DC Kids</a>
                            <a href="" class="list-group-item border-0 text-start p-0">DC Universe</a>
                            <a href="" class="list-group-item border-0 text-start p-0">DC Power Visa</a>
                        </div>
                    </div>
                </div>
                <div class="col-6 bodyBg">
                </div>
            </div>
        </div>
    </div>
    <div class="container-fluid bg_container_foot">
        <div class="container">
            <div class="row py-3 align-items-center">
                <div class="col-2">
                    <button type="button" class="btn btn-outline-primary">SIGN-UP NOW</button>
                </div>
                <div class="col-10 d-flex justify-content-end gap-2">
                    <span class="mx-2 align-self-center text-primary">FOLLOW US</span>
                    <img src="/public/footer-facebook.png" alt="">
                    <img src="/public/footer-twitter.png" alt="">
                    <img src="/public/footer-youtube.png" alt="">
                    <img src="/public/footer-pinterest.png" alt="">
                    <img src="/public/footer-periscope.png" alt="">
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
a {
    font-size: 12px;
    background-color: #00000000;
    color: grey;
}

.bodyBg {
    background-image: url(/public/dc-logo-bg.png);
    min-height: 100%;
    background-repeat: no-repeat;
    background-position: center;
}

.bg_container_foot {
    background-color: #303030;
}

button {
    border-radius: 0;
    color: white;
}

.bg_container {
    background-image: url(/public/footer-bg.jpg);
}
</style>