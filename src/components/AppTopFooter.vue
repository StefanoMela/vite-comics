<script>

export default {
    data () {
        return {

            icons: '',
        }
    }
}

</script>

<template>
    <div class="container-fluid">
        <i>icona</i>
        <i>icona</i>
        <i>icona</i>
        <i>icona</i>
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