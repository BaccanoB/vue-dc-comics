<template>
    <header> 
        <div id="container">
            <img src="../assets/img/dc-logo.png" alt="">
            <nav>
                <ul>
                    <li v-for="(link,index) in links" :key="index">
                        <a href="#" :class="{ active: link.current}">{{ link.text }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
   name:'Header',
   data: function(){
       return {
           links: [
               {
                text: "Cracters",
                current: false
               },
               {
                text: "Comics",
                current: false
               },
               {
                text: "Movies",
                current: false
               },
               {
                text: "TV",
                current: false
               },
               {
                text: "Games",
                current: false
               },
               {
                text: "Collectibles",
                current: false
               },
               {
                text: "Videos",
                current: false
               },
               {
                text: "Fans",
                current: false
               },
               {
                text: "News",
                current: false
               },
               {
                text: "Shop",
                current: false
               }
           ]
       }
   }
}
</script>

<style lang="scss" scoped>
    @import "../style/mixins";
    @import "../style/variable";
    
    header {
        @include flex;
        width: 100%;
        height: 80px;
    }

    #container{
        width: 80%;
        margin: 0 auto;
        @include flex;
        justify-content: space-between;

          img {
        width: 65px;
        }

        nav {
        width: 600px;
        text-align: right;

            ul {
                list-style: none;

                li {
                    display: inline-block;
                    padding: 3px;
                    
                    a{
                        padding: 10px 10px 27px 10px;
                        text-decoration: none;
                        text-transform: $text_style;
                        font-size: $text_size;
                        font-weight: $text_weight;
                        color: black;
                        &.active,
                        &:hover {
                            color: $dc_color;
                            border-bottom: 4px solid $dc_color;
                        }
                    }
                }
            }
        }
    }
</style>
