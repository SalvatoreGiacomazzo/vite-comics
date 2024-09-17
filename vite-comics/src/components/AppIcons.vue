<script>
export default {
    data() {
        return {
         icons: [
            {
                imgSource:'buy-comics-digital-comics.png',
                imgText:'Digital Comics',
                title:'DIGITAL COMICS'
            },
            {
                imgSource:'buy-comics-merchandise.png',
                imgText:'Dc Merchandise',
                title:'DC MERCHANDISE'
            },
            {
                imgSource:'buy-comics-subscriptions.png',
                imgText:'Subscription',
                title:'SUBSCRIPTION'
            },
            {
                imgSource:'buy-comics-shop-locator.png',
                imgText:'Comic Shop Locator',
                title:'COMIC SHOP LOCATOR'
            },
            {
                imgSource:'buy-dc-power-visa.svg',
                imgText:'Dc Power Visa',
                title:'DC POWER VISA'
            },
         ]
        }
    },
    methods: {
        getImageUrl(imgUrl){
         return new URL(`../assets/img/${imgUrl}`, import.meta.url).href
        }
    }
}
</script>


<template>
    <div id="icons">
        <div class="icon" v-for="(icon, index) in icons" :key="index">
            <img :src="getImageUrl(icon.imgSource)" :alt="icon.imgText">
            <h4>{{ icon.title }}</h4>
        </div>
    </div>
</template>

<style></style>