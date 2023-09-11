<script>

export default {
    data () {
        return {

            footerIcons: [{
                
            },]
        }
    }
}

</script>

<template>
    <div class="container-fluid">
        <div class="call__to__action__card">
            <img src="../assets/img/buy-comics-digital-comics.png" alt="">
            <h5>Digital Comics</h5>
        </div>
        <div class="call__to__action__card">
            <img src="../assets/img/buy-comics-merchandise.png" alt="">
            <h5>DC Merchandise</h5>
        </div>
        <div class="call__to__action__card">
            <img src="../assets/img/buy-comics-subscriptions.png" alt="">
            <h5>Subscription</h5>
        </div>
        <div class="call__to__action__card">
            <img src="../assets/img/buy-comics-shop-locator.png" alt="">
            <h5>DC Shop Locator</h5>
        </div>
        <div class="call__to__action__card">
            <img src="../assets/img/buy-dc-power-visa.svg" alt="">
            <h5>DC Power Visa</h5>
        </div>
    </div>
</template>

<style lang="scss" scoped>
.container-fluid{

    width: 100%;
    height: 300px;
    background-color:rgb(0, 130, 249);
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    .call__to__action__card {
    
        display: flex;
        align-items: center;
        justify-content: center;
        color: white;
        text-transform: uppercase;

        img {

            max-width: 100px;
            margin-inline: 1rem;
        }
    }
    
}
</style>