<template>
    <main>
        <div>
             <h2> -- Content Goes Here --</h2>
        </div>
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
        display: flex;
        align-items: center;
        width: 100%;
        height: 80px;
        background-color: #1C1C1C;
        color: white;
    }

    div {
        width: 80%;
        margin: 0 auto;
    }    
</style>