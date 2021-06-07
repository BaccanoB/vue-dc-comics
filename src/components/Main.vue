<template>
    <main>
        <div id="container">
            <section>
             <h2> -- Content Goes Here --</h2>
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
export default {
   name:'Main'
}
</script>

<style lang="scss" scoped>
    @import "../style/general";

    main {
        color: white;
        #container{
            background-color: #1C1C1C;

            section {
                width: 80%;
                height: 80px;
                margin: 0 auto;
                display: flex;
                align-items: center; 
            }  
        }

        #blu_section {
            width: 100%;
            height: 120px;
            background-color: #0282F9; 

            #blu_icon {
                width: 75%;
                margin: 0 auto;
                height: 100%;
                display: flex;
                align-items: center;
                justify-content: space-between;

                div{
                    display: flex;
                    align-items: center;

                    img {
                    height: 50px;
                    }

                    #card_logo {
                    height: 35px;
                    }

                    h4 {
                    text-transform: uppercase;
                    font-weight: 500;
                    font-size: 12px;
                    padding-left: 5px;
                    }
                }

            }
        }
    }
  
</style>