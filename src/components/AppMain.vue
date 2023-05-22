<script>

export default {
    name: "AppMain",
    props: {
        foto: Object,
    },
    data() {
        return {

        }
    }
}
</script>

<template>
    <div class="container-fluid bg_img">
        <div class="container fly_cnt">
            <div class="row">
                <div class="col">
                    <button type="button" class="btn btn-primary fw-bold fly_btn">CURRENT SERIES</button>
                </div>
            </div>
        </div>
    </div>
    <div class="container-fluid bg_grey">
        <div class="container py-4">
            <div class="row text-center">
                <div class="col-2 img-fluid" v-for="pic, c in foto">
                    <img :src="pic.thumb" alt="" class="pic">
                    <span class="fw-bold text-white my-2">{{ pic.series }}</span>
                </div>
                <div col-12>
                    <button type="button" class="btn btn-primary fw-bold">SIGN-UP NOW</button>
                </div>
            </div>
        </div>
    </div>
    <div class="container-fluid  text-bg-primary">
        <div class="container">
            <div class="row justify-content-evenly align-items-center py-4 fw-bold">
                <div class="col-2">
                    <img src="/public/buy-comics-digital-comics.png" alt="" class="imgS">
                    <span class="px-2">DIGITAL COMICS</span>
                </div>
                <div class="col-2">
                    <img src="/public/buy-comics-merchandise.png" alt="" class="imgS">
                    <span class="px-2">DC MERCHANDISE</span>
                </div>
                <div class="col-2">
                    <img src="/public/buy-comics-subscriptions.png" alt="" class="imgS">
                    <span class="px-2">SUBSCRIPTION</span>
                </div>
                <div class="col-2">
                    <img src="/public/buy-comics-shop-locator.png" alt="" class="imgS">
                    <span class="px-2">COMIC SHOP LOCATION</span>
                </div>
                <div class="col-2">
                    <img src="/public/buy-dc-power-visa.svg" alt="" class="imgS">
                    <span class="px-2">DC POWER VISA</span>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
.imgS {
    width: 30px;
    aspect-ratio: 1;
}

.bg_img {
    background-image: url(/public/jumbotron.jpg);
    height: 400px;
}

.fly_cnt {
    position: relative;
    height: 100%;
}

.fly_btn {
    position: absolute;
    top: 95%;
}

.bg_grey {
    background-color: rgb(71, 71, 71);
}

.pic {
    height: 90%;
    width: 100%;
}

span {
    font-size: 12px;
}

button {
    border-radius: 0;
}
</style>