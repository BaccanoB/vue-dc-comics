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
    @import "../style/general";
    
    header {
        width: 100vw;
        height: 80px;
    }

    #container{
        width: 80%;
        margin: 0 auto;
        display: flex;
        justify-content: space-around;
        align-items: center;
    }

    img {
        width: 60px;
    }

    nav {
        width: 60%;
    }

    ul {
        list-style: none;

        li {
            display: inline-block;
            padding: 3px;

            &:hover {
                border-bottom: 2px solid#0282F9;
            }
            
            a{
                padding: 10px;
                text-decoration: none;
                text-transform: uppercase;
                font-size: 10px;
                font-weight: bold;
                color: black;
                &.active,
                &:hover {
                     color: #0282F9;
                }
            }
        }
    }
</style>
