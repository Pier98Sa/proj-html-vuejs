<template>
  <div class="newsletter">
      <div class="container-xl">
          <div class="row">
              <div class="col-5 offset-4 d-flex flex-column align-items-center">
                <h2 class="py-5 fs-2">Sign up to our Newsletter</h2>

                <input type="text" class="w-100">

                <div class="button w-100 py-4">
                    <button type="submit" class="ms_btn ms_btn-green w-100">Subscribe</button>
                </div>

                <p class="pb-4 ">(We do not share your data with anybody, and only use it for its intended purpose)</p>

              </div>

          </div>

      </div>
      
  </div>
</template>

<script>

export default {
    name: 'MyNewsletter',
    
}
</script>

<style lang="scss" scoped>
@import "../../style/variables.scss";

    .newsletter{
        background-image: url(../../assets/newsletter_background.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        background-position:bottom;

        input{
            padding: 10px;
            background-color: $secondaryColorNewsletter;
            border: 1px solid $primaryColorNewsletter;

        }

        p{
          color: $primaryColorNewsletter;  
          font-size: 13px;
        }

    }

</style>