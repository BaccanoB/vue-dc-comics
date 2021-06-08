<template>
  <div class="comics">
      <div id="img_container" >
          <img :src="img" alt="">
          <figcaption> {{ text }} </figcaption>
      </div>
  </div>
</template>

<script>
export default {
    name:"Comics",
    props:{
        img: String,
        text: String
    }
}
</script>

<style lang="scss" scoped>
    .comics {
        width: calc(100% / 6);
        height: 200px;
        padding: 20px;

        #img_container{
            height: 80%;

            img {
            width: 90%;
            
        }
        }

    }
</style> 

