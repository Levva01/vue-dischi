<template>

    <header class="header">

        <div class="img-container">

            <img src="../assets/spotify-logo.png" alt="">

        </div>


    </header>


</template>

<script>
export default {
    name: 'BaseHeader',
    data(){

    },
}
</script>

<style lang="scss" scoped>

    .header{
        height: 6.25rem;
        width: 100%;
        background-color: #2e3a46;
        display: flex;
        align-items: center;
        padding-left: 1.875rem;

        .img-container{
            width: 75px;
            height: 3.75rem;

            img{
                width: 100%;
                height: auto;
            }
        }
        

    }

</style>