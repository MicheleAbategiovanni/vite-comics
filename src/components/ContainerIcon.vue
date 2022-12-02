<template>

    <div class="bg-primary py-5">

        <div class="container">

            <div class="row align-items-center row-cols-1 row-cols-md-3 row-cols-lg-5 gy-5">

                <div class="col" v-for="icon in iconList">
                    <a href="#" class="text-decoration-none text-white">

                        <img :src=icon.img class="img-fluid" width="40" :alt="icon.alt">
                        <span class="ms-2">{{ icon.title }}</span>

                    </a>
                </div>

            </div>

        </div>

    </div>



</template>
  
  
<script>
export default {

    data() {
        return {
            iconList: [
                {
                    title: "DIGITAL COMICS",
                    alt: "Logo digital comics",
                    img: "./img/buy-comics-digital-comics.png",
                },
                {
                    title: "DC MERCHANDISE",
                    alt: "Logo merchandise",
                    img: "./img/buy-comics-merchandise.png",
                },
                {
                    title: "SUBSCRIPTION",
                    alt: "Logo subscriptions",
                    img: "./img/buy-comics-subscriptions.png",
                },
                {
                    title: "COMIC SHOP LOCATOR",
                    alt: "Logo shop locator",
                    img: "./img/buy-comics-shop-locator.png",
                },
                {
                    title: "DC POWER VISA",
                    alt: "Logo power visa",
                    img: "./img/buy-dc-power-visa.svg",
                },
            ]
        }
    }

}
</script>
  
  
  
<style lang="scss">

</style>