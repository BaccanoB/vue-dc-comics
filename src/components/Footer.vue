<template>
    <footer>
        <section id="dc_logo_section">
            <div id="footer_list">
                <div>
                    <h3>Dc comics</h3>
                    <ul>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Video</li>
                        <li>News</li>
                    </ul>
                    <h3>Shop</h3>
                    <ul>
                        <li>Shop DC</li>
                        <li>Shop DC-Collectables</li>
                    </ul>
                </div>
                <div>
                    <h3>DC</h3>
                    <ul>
                        <li>Terms of use</li>
                        <li>Privacy policy</li>
                        <li>Add choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscription</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop help</li>
                        <li>Contact us</li>
                    </ul>
                </div>
                <div>
                    <h3>Sites</h3>
                    <ul>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
                    </ul>
                </div>
            </div>
            <div id="dc_logo">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </section>
        <section id="footer_social_icons">
            <div>
                <div id="button_container">
                    <button>Sign-up now!</button>
                </div>
                <div id="icons_container">
                   <a href="#">Follow us</a>
                   <ul>
                       <li>
                           <i class="fab fa-facebook-f"></i>
                       </li>
                       <li>
                           <i class="fab fa-twitter"></i>
                       </li>
                       <li>
                           <i class="fab fa-youtube"></i>
                       </li>
                       <li>
                           <i class="fab fa-pinterest-p"></i>
                       </li>
                       <li>
                           <i class="fas fa-map-marker-alt"></i>
                       </li>
                    </ul>   
                </div>
            </div>
        </section>
    </footer>
</template>

<script>
export default {
   name:'Footer'
}
</script>

<style lang="scss" scoped>
    @import "../style/variable";
    @import "../style/mixins";

    footer{
        width: 100%;
        height: calc(100vh - 280px);

        #dc_logo_section {
            display: flex;
            width: 100%;
            height: calc(100% - 80px);
            background: url(../assets/img/footer-bg.jpg);
            background-size: cover;
            background-position: top;

            #dc_logo {
            position: relative;
            width: 50%;
            height: 100%;
            overflow: hidden;

            img{
                position: absolute;
                top: -60px;
                height: 450px;
            }
            }
            #footer_list {
            display: flex;
            width: 50%;
            height: 100%;
            padding: 20px;
            margin-left: 120px;
            color: white;

                div {
                margin: 0 10px;
                }

                h3 {
                font-size: 14px;
                text-transform: $text_style;
                }

                ul {
                padding: 10px 0;
                list-style: none;
                font-size: 11px;
                font-weight: $text_weight;
                color: #777777;
                }
            }
        }

        #footer_social_icons {
        @include flex;
        width: 100%;
        height: 80px;
        background-color: #303030;

            div {
                display: flex;
                width: 80%;
                margin: 0 auto;

                #button_container {
                width: 50%;

                button {
                padding: 10px;
                text-transform: $text_style;
                font-size: $text_size;
                background-color: #303030;
                color: white;
                border: 2px solid $dc_color;
                }
                }

                #icons_container{
                width: 50%;
                @include flex;
                justify-content: flex-end;

                    a {
                        margin-right: 10px;
                        text-decoration: none;
                        font-size: 16px;
                        font-weight: $text_weight;
                        text-transform: $text_style;
                        color:  $dc_color;
                    }

                    ul {
                        list-style: none;

                        li {
                            display: inline-block;
                            margin: 0 10px;

                            i {
                                width: 35px;
                                height: 35px;
                                font-size: 25px;
                                border-radius: 50%;
                                line-height: 35px;
                                vertical-align: middle;
                                text-align: center;
                                font-weight: $text_weight;
                                color: #303030;
                                background-color: #777777;
                            }
                        }
                    }
                }  
            }
        }
    }

</style>