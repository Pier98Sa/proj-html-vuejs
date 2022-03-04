<template>
    <div class="hero">
        <img class="img-fluid" src="../assets/homepage-hero-background.jpg" alt="">

        <div class="text-hero my_container">
            <h1>Drive with Avada</h1>
            <p>We offer the finest driving tuition money can buy</p>
        </div>
    </div>
  
</template>

<script>
export default {
    name:'MyHero',

}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

    .hero{
        padding-top: 20px;
        position: relative;

        img{
            width: 100%;
        }

        .text-hero{
            position: absolute;
            top: 50%;
            left: 21%;
            color: $primaryColorHero;

            h1{
                font-size: 3.5em;
            }

            p{
                font-size: 1.5em;
            }

        }
        

    }

</style>