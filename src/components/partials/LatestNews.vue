<template>
  <div class="latest-news">
      <div class="container-xl">
          <div class="row">
              <div class="col">
                  <div class="box d-flex flex-column align-items-center ms_offset">
                      <h2 class="fs-2 fw-bold pt-5">Latest News</h2>

                      <div class="news d-flex">
                          <div class="article w-50">
                              <div class="article-img">
                                <img src="../../assets/blog-choosecar-700x441.jpg" alt="">
                              </div>
                              <div class="article-text text-center">
                                <h2 class="fs-5 pt-2">What Car to Start With?</h2>
                                <h3>February 7th, 2019 <span>| 0 Comments</span></h3>
                                <p class="fs-6">Lorem ipsum dolor sit amet, consectetur adipiscing</p> 
                              </div>
                              
                          </div>
                          <div class="article w-50">
                              <div class="article-img">
                                <img src="../../assets/blogpost-10and2-700x441.jpg" alt="">
                              </div>
                              <div class="article-text text-center">
                                <h2 class="fs-5 pt-2">Avada Driving School Expanding</h2>
                                <h3>February 7th, 2019 | 0 Comments</h3>
                                <p class="fs-6">Lorem ipsum dolor sit amet, consectetur adipiscing</p>
                              </div>
                              
                          </div>
                      </div>

                      <div class="button">
                          <button type="submit" class="ms_btn ms_btn-green ">More from the blog</button>
                      </div>
                  </div>

                    <div class="bottom-box pb-5">
                        <img src="../../assets/latestnews-bottom.png" alt="">
                    </div> 
              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name:'LatestNews'
}
</script>

<style lang="scss" scoped>
@import "../../style/variables.scss";

    .latest-news{
        background-image: url(../../assets/latestnews-background.jpg);
        background-color: $primaryColorNews;
        background-repeat: no-repeat;
        background-size: cover;
        background-position:bottom;
        
    }

    .box{
        background-color: $primaryColorNews;
        border-top: 3px solid $quaternaryColorNews;
        border-top-left-radius: 8px;
        border-top-right-radius: 8px;
        .news{
            .article{
                padding: 50px;

                .article-img{
                    width: 100%;
                    

                    img{
                        width: 100%;
                        
                    }
                }

                .article-text{
                    h2{
                        color:$secondaryColorNews;
                    }
                    h3{
                        font-size: 12px;
                        color: $tertiaryColorNews;

                        span{
                           color:$secondaryColorNews; 
                        }
                    }
                    p{
                        color:$tertiaryColorNews;
                    }
                }
            }
            
            
        }
    }

    .bottom-box{
        img{
            width: 100%;

        }
    }

</style>