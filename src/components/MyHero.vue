<template>
    <div class="hero">
        <img class="img-fluid" src="../assets/homepage-hero-background.jpg" alt="">

        <div class="text-hero">
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
            top: 55%;
            left: 25%;
            color: $primaryColorHero;

        }
        

    }

</style>