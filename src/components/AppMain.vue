<script>

export default {
    name: "AppMain"
}
</script>

<template>
    <div class="container-fluid  text-bg-dark ">
        <div class="container py-4">
            <div class="row">
                <div class="col-4">
                    <span class="fw-bold"> -- > Content goes here -- </span>
                </div>
            </div>
        </div>
    </div>
    <div class="container-fluid  text-bg-primary">
        <div class="container">
            <div class="row justify-content-evenly align-items-center py-4 fw-bold">
                <div class="col-2">
                    <img src="/public/buy-comics-digital-comics.png" alt="">
                    <span class="px-2">DIGITAL COMICS</span>
                </div>
                <div class="col-2">
                    <img src="/public/buy-comics-merchandise.png" alt="">
                    <span class="px-2">DC MERCHANDISE</span>
                </div>
                <div class="col-2">
                    <img src="/public/buy-comics-subscriptions.png" alt="">
                    <span class="px-2">SUBSCRIPTION</span>
                </div>
                <div class="col-2">
                    <img src="/public/buy-comics-shop-locator.png" alt="">
                    <span class="px-2">COMIC SHOP LOCATION</span>
                </div>
                <div class="col-2">
                    <img src="/public/buy-dc-power-visa.svg" alt="">
                    <span class="px-2">DC POWER VISA</span>
                </div>
            </div>
        </div>
    </div>
</template>

<style scoped>
img {
    width: 30px;
    aspect-ratio: 1;
}

span {
    font-size: 12px;
}
</style>