<template>
    <header>
        <div class="navbar-top">
            <div class=" d-flex justify-content-between align-items-center container-xl h-100 ms_fs">
                
                <span>We have a 95% Successful pass Rate!</span>
            
                <span><i class="fa-solid fa-phone-flip me-3"></i>Give us a call to book your tuition! 1-800-555-555</span>
                
                
            </div>
            
        </div>
        <div class="navbar-bottom ">
           <div class="container-xl d-flex justify-content-between align-items-center  h-100">
               <div class="row w-100">
                   <div class="col-4">
                        <a  href="#"><img class="ms_logo" src="../assets/avada-drivers-logo-2x-400x77.png" alt=""></a>
                   </div>

                   <div class="col-8 ">
                       <ul class="d-flex justify-content-around align-items-center">
                            <!--Popolamento dinamico delle voci del menu-->
                            <li v-for="(link,index) in links" :key="index" class="px-3">
                                <a :href="link.url"  @click="menuActive(index)" :class="(index == active) ? 'active':''">{{link.text}}</a>
                            </li>
                            <li class="px-3">
                                    <button class="text-white ms_btn-green">Book Now</button>
                            </li>
                        </ul>
                   </div>
               </div>

           </div>
            
                    
               
        </div>         
    </header>
  
</template>

<script>
export default {
    name:'MyHeader',
    //cambio dinamico della voce del menu con la classe active al click
    methods: {
        menuActive(index){
            this.active = index;
        }
    },
    data() {
        return {
        active: 0,
        links: [
                {
                    text: "Home",
                    url: "#"
                },
                {
                    text: "About",
                    url: "#"
                },
                {
                    text: "Prices",
                    url: "#"
                },
                {
                    text: "Courses",
                    url: "#"
                },
                {
                    text: "Locations",
                    url: "#"
                },
                {
                    text: "Blog",
                    url: "#"
                }
            ],
        }
    }

}
</script>

<style lang="scss" scoped>

@import "../style/variables.scss";

    header{
        position: fixed;
        width: 100%;
        top: 0;
        left: 0;
        z-index: 999;

    }
    .navbar-top{
        height: 40px;
        background-color: $primaryColorHeader;
        color: $quaternaryColorHeader;

        .ms_fs{
            font-size: 14px;
        }
    }
    .navbar-bottom{
        height: 100px;
        background-color: $secondaryColorHeader;
        color: $tertiaryColorHeader;
        
        .ms_logo{
            width: 250px;
        }

        li{
            display: inline;

            a{
                padding-bottom:5px ;
                text-decoration: none;
                text-transform: uppercase;
                font-size: 14px;
                color: $tertiaryColorHeader;
                

                &.active,
                &:hover{
                color: $quinaryColorHeader;
                border-bottom: 2px solid $quinaryColorHeader;
                }
            
            }
        }
    }

    
</style>