<template>
  <div class="Statistics">
    <div class="container-xl ms_offset-4">
      <div class="row">
        <div class="col-4">
          <div class="box d-flex flex-column align-items-center">
             <div id="circle-loader-wrap">
              <div class="center d-flex justify-content-center align-items-center">
                <span>95%</span>
              </div>
              <div class="inner">
                <div class="left-wrap">
                    <div class="loader"></div>
                </div>
                <div class="right-wrap">
                    <div class="loader"></div>
                </div>
              </div>
                
            </div>

            <span>Pass Rate</span>
          </div>
          

        </div>

        <div class="col-4">
          <div class="box d-flex flex-column align-items-center">
             <div id="circle-loader-wrap">
              <div class="center d-flex justify-content-center align-items-center">
                <span>95%</span>
              </div>
              <div class="inner">
                <div class="left-wrap">
                    <div class="loader"></div>
                </div>
                <div class="right-wrap">
                    <div class="loader"></div>
                </div>
              </div>
                
            </div>

            <span>Pass Rate</span>
          </div>

          
        </div>

        <div class="col-4">
          <div class="box d-flex flex-column align-items-center">
             <div id="circle-loader-wrap">
              <div class="center d-flex justify-content-center align-items-center">
                <span>95%</span>
              </div>
              <div class="inner">
                <div class="left-wrap">
                    <div class="loader"></div>
                </div>
                <div class="right-wrap">
                    <div class="loader"></div>
                </div>
              </div>
                
            </div>

            <div class="big">
              <div class="inner-big">
              </div>

            </div>

            <span>Pass Rate</span>
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
  .box{
    border-top: 5px solid #8ec67a ;
    border-radius: 12px;
    background-color: #fff;
    height: 500px;

    
  }

  //preso spunto da questa risposta su stackoverflow https://stackoverflow.com/a/48372346

  //creo il cerchio che mi farà da wrap
  #circle-loader-wrap {
  overflow: hidden;
  position: relative;
  width: 200px;
  height: 200px;
  box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.1)inset;
  background-color: grey;
  border-radius: 200px;

}
#circle-loader-wrap .center{
  background-color:white;
  width: 170px;
  height: 170px;
  border-radius:50%;
  position:absolute;
  top:15px;
  left:15px;
  color:black;
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
        border-radius: 1000px;
        background-color: green;
    }

    #circle-loader-wrap .left-wrap {
        left: 0;
    }

    #circle-loader-wrap .left-wrap .loader {
        border-top-left-radius: 0;
        border-bottom-left-radius: 0;
        transform-origin: 0 50% 0;
        animation: loading-left 5s forwards linear;
    }

    #circle-loader-wrap .right-wrap {
        left: 50%;
    }

    #circle-loader-wrap .right-wrap .loader {
        left: -100%;
        border-bottom-right-radius: 0;
        border-top-right-radius: 0;
        transform-origin: 100% 50% 0;
        animation: loading-right 5s forwards linear;
    }

    @keyframes loading-left {
        0% {
            transform: rotate(0deg);
        }
        25%, 100% {
            transform: rotate(180deg);
        }
    }

    @keyframes loading-right {
        0%, 25% {
            transform: rotate(0deg);
        }
        50%, 100% {
/*          the following is for the second half of the cicrle */
/*          180deg means one half of the cicle or 50% of the cicle */
/*          So, 1% is gonna be 180/50 = 3.6deg */
/*          If you want 68%, then you have 18% left for the second half of the circle */
/*          To get 18%: 18x3.6 = 64.8deg */
            transform: rotate(64.8deg);
/*          Note: The transformation will happen between 25% and 50% of the total time which is 5 seconds in this case; So, it's gonna take 1.25 seconds. */
/*          In other words, it will take the same amount of time as for the first half of the circle which will make the transformation in the second half appear to be slower because it has the same time to cover a much shorter distance */
/*          Between 50% and 100% nothing happens. */
/*          That's your "pause" in this animation although technically it's not a pause. */
        }
    }
</style>