<template>
    <div id="hero" class=" d-flex justify-content-center">
        <img src="../assets/homepage-hero-background.jpg" alt="">

        <div class="text-hero container-xl">
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

    #hero{
        padding-top: 20px;
        position: relative;
        img{
            object-fit: cover;
            width: 100%;
        }
        .text-hero{
            position: absolute;
            top: 50%;
            color: $primaryColorHero;

            h1{
                font-size: 3.7em;
            }

            p{
                font-size: 1.2em;
            }

        }
        

    }

</style>