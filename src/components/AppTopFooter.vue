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
        <i>Digital Comics</i>
        <i>DC Merchandise</i>
        <i>Subscription</i>
        <i>Comic Shop Locator</i>
        <i>DC Power Visa</i>
    </div>
</template>

<styl lang="scss">
.container-fluid{

    width: 100%;
    height: 300px;
    background-color: aqua;

    display: flex;
    justify-content: space-evenly;
    align-items: center;

    i {

        background-color: black;
        color: white;
        padding: 10px;
    }
}
</styl>