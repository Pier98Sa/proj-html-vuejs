<template>
    <div class="CTA">
        <div class="my_container d-flex justify-content-between align-items-center py-5">
            <div >
                <h2 class="fw-bold">Start Learning to Drive Today</h2>
                <p>Give us a call to schedule your first driving lesson</p>
            </div>
            <div>
                <span class="fs-3" ><i class="fa-solid fa-phone-flip me-3"></i>1-800-555-555</span>
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