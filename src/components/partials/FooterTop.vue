<template>
  <div class="footer-top">
      <div class="container-xl">
          <div class="row">
              <div class="col-3">
                  <div class="box-logo">
                      <img src="../../assets/avada-drivers-logo-2x-400x77.png" alt="">
                      <p>Avada Driving School is the right choice for experienced drivers looking for a refresher course, or the brand new driver wanting to pass first time.</p>
                  </div>

              </div>

              <div class="col-3">   
                <div class="contacts">
                    <h2>Contact details</h2>

                    <ul>
                        <li><i class="fa-solid fa-house-chimney"></i> 12345 North Main Street,New York, NY 555555</li>
                        <li><i class="fa-solid fa-phone-flip"></i> 1.800.555.6789</li>
                        <li><i class="fa-solid fa-envelope"></i> info@your-domain.com</li>
                        <li><i class="fa-solid fa-link"></i> Theme-Fusion.com</li>
                    </ul>
                </div>
              </div>

              <div class="col-3">

              </div>

              <div class="col-3">
                  <img src="../../assets/footer-ad-grid.png" alt="">
                  <button class="ms_btn ms_btn-green">Book Now</button>
              </div>

          </div>

      </div>

  </div>
</template>

<script>
export default {
    name: 'FooterTop'
}
</script>

<style lang="scss" scoped>
@import "../../style/variables.scss";
    .footer-top{
        background-image: url(../../assets/footer-background-color.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        background-position:bottom;

        .box-logo{
            img{
                width: 100%;
                padding: 0 10px 0 10px;
            }
            p{
                color: $primaryColorFooterTop;
            }
        }

        .contacts{
            h2{
                color: $secondaryColorFooterTop;
            }

            li{
                list-style: none;
                color: $primaryColorFooterTop;
            }
        }
    }

</style>