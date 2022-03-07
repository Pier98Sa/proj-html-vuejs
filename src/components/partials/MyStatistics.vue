<template>
  <div class="Statistics">
    <div class="container-xl ms_offset-4">
      <div class="row">
        <div class="col-4 ">
          <div class="box d-flex flex-column align-items-center p-5">

            <!--Statistics 1-->
            <div id="circle-loader-wrap">

              <div class="center d-flex justify-content-center align-items-center">
                <span class="fs-1">95%</span>
              </div>

              <div class="inner">
                <div class="left-wrap">
                    <div class="loader my-95"></div>
                </div>

                <div class="right-wrap">
                    <div class="loader my-95"></div>
                </div>
              </div>
                
            </div>

            <span class="py-5">Pass Rate</span>
          </div>
          

        </div>

        <div class="col-4">
          <div class="box d-flex flex-column align-items-center p-5">

            <!--Statistics 2-->
            <div id="circle-loader-wrap">
              
              <div class="center d-flex justify-content-center align-items-center">
                <span class="fs-1">100%</span>
              </div>
              
              <div class="inner">
                <div class="left-wrap">
                    <div class="loader my-100"></div>
                </div>
                <div class="right-wrap">
                    <div class="loader my-100"></div>
                </div>
              </div>
                
            </div>

            <span class="py-5">Referral rate</span>
          </div>

          
        </div>

        <div class="col-4">
          <div class="box d-flex flex-column align-items-center p-5">
            <!--Statistics 3-->
             <div id="circle-loader-wrap">
              <div class="center d-flex justify-content-center align-items-center">
                <span class="fs-1">0%</span>
              </div>
              <div class="inner">
                <div class="left-wrap">
                    <div class="loader my-0"></div>
                </div>
                <div class="right-wrap">
                    <div class="loader my-0"></div>
                </div>
              </div>
                
            </div>

            <span class="py-5">Accident Rate</span>
          </div>

          
        </div>

      </div>

    </div>
  </div>
</template>

<script>
export default {
  name:'MyStatistics'

}
</script>

<style lang="scss" scoped>
@import "../../style/variables.scss";
  .box{
    border-top: 5px solid $secondaryColorStat ;
    border-radius: 12px;
    background-color: $primaryColorStat;
    box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.1);

    span{
      color: $quaternaryColorStat;
      text-transform: uppercase;
      font-size: 18px;
    }
  }

  //preso spunto da questa risposta su stackoverflow https://stackoverflow.com/a/48372346

  //creo il cerchio che mi farà da wrap
  #circle-loader-wrap {
    overflow: hidden;
    position: relative;
    width: 200px;
    height: 200px;
    background-color: $tertiaryColorStat;
    border-radius: 50%;

  }
  #circle-loader-wrap .center{
    background-color:$primaryColorStat;
    width: 170px;
    height: 170px;
    border-radius:50%;
    position:absolute;
    top:15px;
    left:15px;
    color:$quaternaryColorStat;
    z-index:998;
  }

  .inner{
    position:absolute;
    height:100%;
    width:100%;
    top:0;
    left:0;
    transform: rotate(180deg);
  }
  .inner div{
    overflow: hidden;
    position: absolute;
    width: 50%;
    height: 100%;
  }

  #circle-loader-wrap .loader {
    position: absolute;
    left: 100%;
    top: 0;
    width: 100%;
    height: 100%;
    background-color: $secondaryColorStat;
  }

  #circle-loader-wrap .left-wrap {
    left: 0;
  }
  #circle-loader-wrap .right-wrap {
      left: 50%;
    }


  //classi per cambiare il caricamento degli spin

  //per il 95%

  #circle-loader-wrap .left-wrap  .my-95 {
    transform-origin: 0 50% 0;
    animation: loading-left-95 2s forwards linear;
  }
   #circle-loader-wrap .right-wrap .my-95 {
    left: -100%;
    transform-origin: 100% 50% 0;
    animation: loading-right-95 2s forwards linear;
  }

  @keyframes loading-left-95 {
    0% {
      transform: rotate(0deg);
    }
    25%, 100% {
      transform: rotate(180deg);
    }
  }

  @keyframes loading-right-95 {
    0%,25% {
      transform: rotate(0deg);
    }
    50%, 100% {
      transform: rotate(160deg);
    }
  }

  //per il 100%

    #circle-loader-wrap .left-wrap .my-100 {
    transform-origin: 0 50% 0;
    animation: loading-left-100 2s forwards linear;
    }

  
  #circle-loader-wrap .right-wrap .my-100 {
    left: -100%;
    transform-origin: 100% 50% 0;
    animation: loading-right-100 2s forwards linear;
  }

  @keyframes loading-left-100 {
    0% {
      transform: rotate(0deg);
    }
    25%, 100% {
      transform: rotate(180deg);
    }
  }

  @keyframes loading-right-100 {
    0%,25% {
      transform: rotate(0deg);
    }
    50%, 100% {
      transform: rotate(180deg);
    }
  }

  //per il 0%

  #circle-loader-wrap .left-wrap .my-0 {
    transform-origin: 0 50% 0;
    animation: loading-left-0 2s forwards linear;
  }

  #circle-loader-wrap .right-wrap .my-0 {
    left: -100%;
    transform-origin: 100% 50% 0;
    animation: loading-right-0 2s forwards linear;
  }

  @keyframes loading-left-0{
    0% {
      transform: rotate(0deg);
    }
    25%, 100% {
      transform: rotate(4deg);
    }
  }

  @keyframes loading-right-0 {
    0%,25% {
      transform: rotate(0deg);
    }
    50%, 100% {
      transform: rotate(0deg);
    }
  }

</style>