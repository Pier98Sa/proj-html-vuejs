<template>
  <div class="box d-flex flex-column align-items-center ms_offset-5 ">
        <div class="img-box p-5">
            <img :src="require('../../assets/instructor' + (instructor.photo))" :alt="instructor.name">
        </div>

        <h3>{{instructor.name}}</h3>

        <div class="social-box pt-2">
            <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
            <a href="#"><i class="fa-brands fa-twitter px-4"></i></a>
            <a href="#"><i class="fa-brands fa-instagram"></i></a>
        </div>
        
        <div class="description p-4 text-center">
            <p>{{instructor.description}}</p>
        </div>

    </div>
</template>

<script>
export default {
    name: 'InstructorsCard',
    props:{
        instructor: Object,
    }
}
</script>

<style lang="scss" scoped>
@import "../../style/variables.scss";

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

                    &:hover{
                        transform: scale(1.1,1.1);
                        box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.1);
                    }
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

</style>