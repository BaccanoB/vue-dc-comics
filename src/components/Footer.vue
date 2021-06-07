<template>
    <footer>
        <section id="dc_logo_section">
            <div id="footer_list"></div>
            <div id="dc_logo">
                <img src="../assets/img/dc-logo-bg.png" alt="">
            </div>
        </section>
        <section></section>
    </footer>
</template>

<script>
export default {
   name:'Footer'
}
</script>

<style lang="scss" scoped>
    @import "../style/general";

    footer{
        width: 100vw;
        height: calc(100vh - 200px);
    }

    #dc_logo_section {
        display: flex;
        width: 100%;
        height: calc(100% - 150px);
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
            width: 50%;
            height: 100%;
        }
    }
</style>