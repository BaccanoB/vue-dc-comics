<template>
    <main>
        <div id="container">
            <div id="jumbotron">
                <button>Current series</button>
            </div>
            <section>
                <Comics
                    v-for="(comic,index) in comics"
                    :key="index"
                    :img="comic.thumb"
                    :text="comic.series"
                />
                <button>Load More</button>
            </section>
        </div>
        <section id="blu_section">
            <div id="blu_icon">
                <div>
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="#">
                    <h4>digital comics</h4>
                </div>
                <div>
                    <img src="../assets/img/buy-comics-merchandise.png" alt="#">
                    <h4>dc merchandise</h4>
                </div>
                <div>
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="#">
                    <h4>subscription</h4>
                </div>
                <div>
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="#">
                    <h4>comic shop locator</h4>
                </div>
                <div>
                    <img id="card_logo" src="../assets/img/buy-dc-power-visa.svg" alt="#">
                    <h4>dc power visa</h4>
                </div>
            </div>
        </section>
    </main>
</template>

<script>
    import Comics from './Comics';

    export default {
        name:'Main',
        components:{
        Comics:Comics
        },
        data:function (){
        return {
            comics:[
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
                        "price": "$19.99",
                        "series": "Action Comics",
                        "type": "comic book"
                    },
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
                        "price": "$3.99",
                        "series": "American Vampire 1976",
                        "type": "comic book"
                    },
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
                        "price": "$16.99",
                        "series": "Aquaman",
                        "type": "graphic novel"
                    },
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
                        "price": "$2.99",
                        "series": "Batgirl",
                        "type": "comic book"
                    },
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                        "price": "$3.99",
                        "series": "Batman",
                        "type": "comic book"
                    },
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
                        "price": "$2.99",
                        "series": "Batman Beyond",
                        "type": "comic book"
                    },
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
                        "price": "$3.99",
                        "series": "Batman/Superman",
                        "type": "comic book"
                    },
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
                        "price": "$4.99",
                        "series": "Batman/Superman Annual",
                        "type": "comic book"
                    },
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
                        "price": "$5.99",
                        "series": "Batman: The Joker War Zone",
                        "type": "comic book"
                    },
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
                        "price": "$6.99",
                        "series": "Batman: Three Jokers",
                        "type": "comic book"
                    },
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
                        "price": "$4.99",
                        "series": "Batman: White Knight Presents: Harley Quinn",
                        "type": "comic book"
                    },
                    {
                        "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
                        "price": "$16.99",
                        "series": "Catwoman",
                        "type": "graphic novel"
                    }
                ]
            }
        }
    }
</script>

<style lang="scss" scoped>
    @import "../style/variable";
    @import "../style/mixins";

    main {
        color: white;
        #container{
            background-color: #1C1C1C;

            #jumbotron {
                position: relative;
                height: 300px;
                background-image: url(../assets/img/jumbotron.jpg);
                background-size: cover;

                button {
                    position: absolute;
                    top: calc(100% - 20px);
                    left: 150px;
                    color: white;
                    background-color: $dc_color;
                    border: 1px solid $dc_color;
                    padding: 10px;
                    text-transform: $text_style;
                    font-weight: $text_weight;
                }
            }

            & > section {
                @include flex;
                justify-content: space-around;
                flex-wrap: wrap;
                width: 80%;
                margin: 0 auto;
                padding: 20px 0;

                button {
                    color: white;
                    background-color: $dc_color;
                    border: 1px solid $dc_color;
                    padding: 5px 30px;
                    text-transform: $text_style;
                    font-size: $text_size;
                    font-weight: $text_weight;
                }
            } 
        }

        #blu_section {
            width: 100%;
            height: 120px;
            background-color: $dc_color; 

            #blu_icon {
                width: 75%;
                margin: 0 auto;
                height: 100%;
                @include flex;
                justify-content: space-between;

                div{
                    @include flex;

                    img {
                    height: 50px;
                    }

                    #card_logo {
                    height: 35px;
                    }

                    h4 {
                    text-transform: $text_style;
                    font-weight: 500;
                    font-size: $text_size;
                    padding-left: 5px;
                    }
                }

            }
        }
    }
  
</style>