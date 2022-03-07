<template>
    <footer>
        <MyNewsletter />
        <FooterTop />
        
        <div class="footer-bottom">
            
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
    }

}
</script>

<style lang="scss" scoped>
@import "../style/variables.scss";

    .footer-bottom{
        background-color: $primaryColorFooterBottom;
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