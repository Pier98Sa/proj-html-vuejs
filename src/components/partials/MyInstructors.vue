<template>
<div class="Instructors mt-5">
    <div class="container-xl">
      <div class="row align-items-center">
          <div class="col-9">
              <h2 class="fs-1">Your Instructors</h2>
              <p class="fs-4 pt-4 my_p-color">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc ultrices auctor sapien id cursus. Aliquam maximus turpis in vehicula semper.</p>
          </div>

          <div class="col-3">
              <button type="submit" class="ms_btn ms_btn-green w-100">More about us</button>
          </div>
      </div>

      <div class="row mt-5">
          <div class="col-4">
              <div class="box d-flex flex-column align-items-center ms_offset-5 ">
                    <div class="img-box p-5">
                        <img src="../../assets/instructor-mikehart.jpg" alt="Mike Hart">
                    </div>

                    <h3>Mike Hart</h3>

                    <div class="social-box pt-2">
                        <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
                        <a href="#"><i class="fa-brands fa-twitter px-4"></i></a>
                        <a href="#"><i class="fa-brands fa-instagram"></i></a>
                    </div>
                    
                    <div class="description p-4 text-center">
                        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                    </div>

              </div>
          </div>

          <div class="col-4">
              <div class="box d-flex flex-column align-items-center ms_offset-5">
                  <div class="img-box p-5">
                        <img src="../../assets/instructor-johnsmith.jpg" alt="Mike Hart">
                    </div>

                    <h3>John Smith</h3>

                    <div class="social-box pt-2">
                        <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
                        <a href="#"><i class="fa-brands fa-twitter px-4"></i></a>
                        <a href="#"><i class="fa-brands fa-instagram"></i></a>
                    </div>
                    
                    <div class="description p-4 text-center">
                        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                    </div>
              </div>
          </div>

          <div class="col-4">
              <div class="box d-flex flex-column align-items-center ms_offset-5">
                  <div class="img-box p-5">
                        <img src="../../assets/instructor-angelahart.jpg" alt="Mike Hart">
                    </div>

                    <h3>Angela Hart</h3>

                    <div class="social-box pt-2">
                        <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
                        <a href="#"><i class="fa-brands fa-twitter px-4"></i></a>
                        <a href="#"><i class="fa-brands fa-instagram"></i></a>
                    </div>
                    
                    <div class="description p-4 text-center">
                        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
                    </div>

              </div>
          </div>

      </div>
  </div>
</div>
  
</template>

<script>
export default {
    name: 'MyInstructors',
}
</script>

<style lang="scss" scoped>
@import "../../style/variables.scss";
    .Instructors{
        background-color: $secondaryColorInstr;
        
        .my_p-color{
            color:$primaryColorInstr;
        }

        .box{
            border-top: 4px solid $tertiaryColorInstr;
            background-color: $secondaryColorInstr;
            border-radius: 12px;
            box-shadow: 0px 0px 20px $primaryColorInstr;
            

            .img-box{

                img{
                    width: 100%;
                    height: 100%;
                    object-fit: cover;
                }
            }

            .social-box{
                a{
                    color: $primaryColorInstr;
                }
            }

            .description{
                color: $primaryColorInstr;
            }
        }
    }

</style>