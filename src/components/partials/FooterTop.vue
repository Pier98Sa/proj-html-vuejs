<template>
  <div class="footer-top">
      <div class="container-xl">
          <div class="row py-5 align-items-center">
              <div class="col-3">
                  <div class="box-logo p-4">
                      <img src="../../assets/avada-drivers-logo-2x-400x77.png" alt="">
                      <p class="pt-3">Avada Driving School is the right choice for experienced drivers looking for a refresher course, or the brand new driver wanting to pass first time.</p>
                  </div>

              </div>

              <div class="col-3">   
                <div class="contacts p-4">
                    <h2>Contact details</h2>
                    <ul class="fa-ul">
                        <li class="py-1"><span class="fa-li"><i class="fa-solid fa-house-chimney"></i></span>12345 North Main Street,New York, NY 555555</li>
                        <li  class="py-1"><span class="fa-li"><i class="fa-solid fa-phone-flip"></i></span>1.800.555.6789</li>
                        <li  class="py-1"><span class="fa-li"><i class="fa-solid fa-envelope"></i></span>info@your-domain.com</li>
                        <li  class="py-1"><span class="fa-li"><i class="fa-solid fa-link"></i> </span>Theme-Fusion.com</li>
                    </ul>
                </div>
              </div>

              <div class="col-3">
                  <div class="courses p-4">
                    <h2>Courses</h2>
                    <ul class="fa-ul">
                        <li v-for="(course,index) in courses" :key="index" class="py-1">
                            <a :href="course.link"> <span class="fa-li"><i class="far fa-arrow-alt-circle-right"></i></span> {{course.name}}</a>
                        </li>
                    </ul>
                  </div>
                  

              </div>

              <div class="col-3">
                  <div class="ads p-4">
                    <img  src="../../assets/ad.png"  alt=""> <!--Immagine non funzionante-->
                    <button class="ms_btn ms_btn-green">Book Now</button>
                  </div>
                  
              </div>

          </div>

      </div>

  </div>
</template>

<script>
export default {
    name: 'FooterTop',
    data(){
        return{
            courses:[
                {
                    name: 'Pass Plus',
                    link: '#'
                },
                {
                    name: 'Intensive Course',
                    link: '#'
                },
                {
                    name: 'Automatic',
                    link: '#'
                },
                {
                    name: 'Instructor Training',
                    link: '#'
                }
            ]
        }
    }
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

            }
            p{
                color: $primaryColorFooterTop;
                font-size: 13px;
            }
        }

        .contacts{
            h2{
                color: $secondaryColorFooterTop;
            }

            li{
                list-style: none;
                color: $primaryColorFooterTop;
                font-size: 13px;
            }
        }

        .courses{
            h2{
                color: $secondaryColorFooterTop;
            }

            li{
                list-style: none;
                a{
                  color: $tertiaryColorFooterTop;
                  text-decoration: none;  
                  font-size: 17px;
                }
                
            }
        }

        
    }

</style>