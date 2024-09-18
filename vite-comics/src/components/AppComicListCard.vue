<script>
export default {
    data() {
        return {

        }
    },
  props:{
    comic: {
        type: Object,
        required: true
    }
      },
       props:{
      comicName:{
      required: true,
      type: String
               },

      comicImg: {
        required: true,
        type: String
      }

  }

}

</script>


<template>
<div class="card">
  <img :src="comicImg" alt="">
  <h3>{{ comicName }}</h3>

</div>

</template>

<style scoped lang="scss">


.card img{
  max-height:100%;
  display:block;
  max-width:100%;
  
}

</style>