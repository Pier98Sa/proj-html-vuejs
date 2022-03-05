<template>
    <div class="CTA">
        <div class="container-xl py-5">
            <div class="row">
                <div class="col-8">
                    <h2 class="fw-bold fs-1">Start Learning to Drive Today</h2>
                    <p class="fs-5">Give us a call to schedule your first driving lesson</p>
                </div>
                <div class="col-4">
                    <span class="fs-3 text-end" ><i class="fa-solid fa-phone-flip me-3"></i>1-800-555-555</span>
                </div>
            </div>
            

        </div>
        
    </div>
  
</template>

<script>
export default {
    name: 'MyCTA'
}
</script>

<style lang="scss" scoped>
@import "../../style/variables.scss";

    .CTA{
        background-image: url(../../assets/horizontal-cta-background.jpg);
        background-repeat: no-repeat;
        background-position:bottom;
        background-size: cover;
        color: $primaryColorCTA;
        
    }

</style>