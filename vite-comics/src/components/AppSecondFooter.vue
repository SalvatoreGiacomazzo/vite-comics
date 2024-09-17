<script>
export default {
    data() {
        return {
          socials: [
            {
                id:'1',
                socialUrl:'footer-facebook.png',
                alt:'facebook'
            },
            {
                id:'2',
                socialUrl:'footer-periscope.png',
                alt:'periscope'
            },
            {
                id:'3',
                socialUrl:'footer-pinterest.png',
                alt:'pinterest'
            },
            {
                id:'4',
                socialUrl:'footer-twitter.png',
                alt:'twitter'
            },
            {
                id:'5',
                socialUrl:'footer-youtube.png',
                alt:'youtube'
            },
          ]
        }
    },
    methods:{
        getSocialImg(socialUrl){
            return new URL(`../assets/img/${socialUrl}`, import.meta.url).href
        }
    }
}
</script>


<template>
    <footer id="second-footer">
        <button>SIGN UP NOW!</button>
        <div id="second-footer-left">
            <h2>FOLLOW US</h2>
        <div id="sf-icons" v-for="(social, id) in socials" :key="social.id" >
            
            <img :src="getSocialImg(social.socialUrl)" :alt="social.alt">
           
        </div>
        </div>
    </footer>
</template>

<style scoped>
#second-footer-left{
    display:flex;
}
h2{
    color:dodgerblue;
}
</style>