<template>
  <div class="Testimonials d-flex align-items-center " >
      <div class="container-xl">
          <div class="row ">
                <div class="offset-3 col-6 d-flex flex-column align-items-center py-5">
                    <div class="title text-center">
                        <h2 class="fs-1">Testimonials</h2>
                        <p class="fs-4">Here’s what our happy drivers had to say about our services:</p>
                    </div>

                    <!--photo-->
                    <div class="photo-box py-4">
                        <img src="../../assets/testimonial-sophia.png" alt="">
                    </div>
 
                    <!--description-->
                    <div class="description text-center fs-5">
                        <p>Avada Driving School really helped build my confidence behind the wheel and with driving in general, and they got me a first time pass! Highly recommended.</p>
                    </div>

                    <!--name-->
                    <h2 class="fs-5 name">Sophia Jones</h2>

                    <!--circle-->
                    <div class="circle-box py-3">
                        <div class="circle active"></div>
                        <div class="circle"></div>
                        <div class="circle"></div>
                        <div class="circle"></div>
                        <div class="circle"></div>
                    </div>
                </div>
          </div>

        </div>

  </div>
</template>

<script>
export default {
    name: 'MyTestimonials',
    data(){
        return{
            active:0,
            testimonials:[
                {
                    name: 'Sophia Jones',
                    photo: 'sophia.png'
                },
                {
                    name: 'Harold Green',
                    photo: 'harold.png'
                },
                {
                    name: 'Grant Harvey',
                    photo: 'grant.png'
                },
                {
                    name: 'Kate Lewis',
                    photo: 'kate.png'
                },
                {
                    name: 'Kelly Johnson',
                    photo: 'kelly.png'
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../style/variables.scss";

    .Testimonials{
        background-image: url(../../assets/testimonial-background.jpg);
        background-repeat: no-repeat;
        background-size: cover;
        background-position:bottom;
        height: 860px;
        z-index: -1;
        
        .title{
            p{
               color:$primaryColorInstr; 
            }
            
        }

        .photo-box{
            width: 150px;

            img{
                width: 100%;
                object-fit: cover;
            }
        }

        .description{
            color:$primaryColorInstr; 
        }

        .circle-box{


            .circle {
                width: 10px;
                height: 10px;
                background-color: transparent;
                border: 1px solid $primaryColorTestimonials;
                border-radius: 50%;
                display: inline-block;
                margin: 0 5px;
            }

            .circle.active {
                background-color: $primaryColorTestimonials;
            }
        }

        .name{
           color:$primaryColorInstr;  
        }
    }


</style>