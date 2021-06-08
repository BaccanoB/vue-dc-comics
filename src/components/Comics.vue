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

 @import "../style/variable";
    .comics {
        width: calc(100% / 6);
        height: 300px;
        padding: 10px;

        #img_container{
            height: 80%;

            img {
            width: 90%;
            }

            figcaption {
                text-transform: $text_style;
                font-size: $text_size;
                font-weight: bold;
            }
        }

    }
</style> 

