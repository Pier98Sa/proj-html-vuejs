<template>
    <footer>
        
        <MyNewsletter />
        <FooterTop :courses="courses" />
        
        <div class="footer-bottom">
            <div class="ToTop d-flex align-items-center justify-content-center">
                <a class="text-white" href="#hero"><i class="fa-solid fa-chevron-up"></i> </a>
            </div>
            
            <div class="container-xl py-5">
                <div class="row align-items-center justify-content-center">
                    <div class="col-10 d-flex align-item-center">
                        <div>
                            <p>© Copyright 2012 - 2022 | Avada Theme by <span>ThemeFusion</span>  | All Rights Reserved | Powered by <span>WordPress</span> </p>
                        </div> 
                    </div>

                    <div class="col-2 d-flex align-item-center">
                        <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
                        <a href="#"><i class="fa-brands fa-twitter"></i></a>
                        <a href="#"><i class="fa-brands fa-youtube"></i></a>
                        <a href="#"><i class="fa-brands fa-instagram"></i></a>

                    </div>

                </div>

            </div>
        </div>
        
    </footer>
  
</template>

<script>
import MyNewsletter from './partials/MyNewsletter.vue'
import FooterTop from './partials/FooterTop.vue'

export default {
    name:'MyFooter',
    components:{
       MyNewsletter,
       FooterTop
    },
    props: {
        courses : Array
    }

}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

    .footer-bottom{
        background-color: $primaryColorFooterBottom;
        .ToTop{
            position: fixed;
            bottom: 0;
            right: 30px;
            height: 35px;
            width: 50px;
            background-color: $primaryColorFooterBottom;
            font-size: 25px; 
        }
        p{
            color: $tertiaryColorFooterBottom;
            font-size: 12px;
            margin:0px;

            span{
                color: $secondaryColorFooterBottom;
            }
        }

        a{
            color: $quaternaryColorFooterBottom;
            padding: 0 10px 0 10px;
            font-size: 12px;
            margin:0px;
        }
    }
</style>