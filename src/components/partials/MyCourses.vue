<template>
  <div class="course">
      <div class="container-xl pb-5">
            <div class="row align-items-center">
                <div class="col-4">
                    <div class="box text-center position-relative ms_offset-2">
                        <div class="px-3">
                            <h3 class="pt-5 fs-2">Courses</h3>
                            <p class="p-4">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc ultrices auctor sapien id cursus. Aliquam maximus turpis in vehicula semper.</p>
                            
                            <div class="pb-5">
                                <button type="submit" class="ms_btn ms_btn-green">Course information</button>
                            </div>
                        </div>
                            
                        <img class="new-img" src="../../assets/new-corner.jpg" alt="new">
                    </div> 

                </div>

                <div class="col-8">
                    <div class="row ">
                        <div class="col-4 ">
                            <div class="p-5">
                                <div class="img-box">
                                    <img src="../../assets/courses-passplus-400x399.jpg" alt="pass plus">
                                </div>
                            

                                <h4 class="text-center ms_text-color fs-5 py-2">Pass Plus</h4>

                                <div class="text-center">
                                    <button class="ms_btn ms_btn-grey" type="submit">Lean More</button>
                                </div>

                            </div>
                           
                            
                        </div>

                        <div class="col-4 ">
                            <div class="p-5">
                                 <div class="img-box">
                                    <img src="../../assets/course-intensive-400x399.jpg" alt="pass plus">
                                </div>
                            

                                <h4 class="text-center ms_text-color fs-5 py-2">Intensive Course</h4>

                                <div class="text-center">
                                    <button class="ms_btn ms_btn-grey" type="submit">Lean More</button>
                                </div>
                            </div>
                           

                        </div>

                        <div class="col-4 ">
                            <div class="p-5">
                                <div class="img-box">
                                    <img src="../../assets/courses-instructor-400x400.jpg" alt="pass plus">
                                </div>
                            

                                <h4 class="text-center ms_text-color fs-5 py-2">Instructors</h4>

                                <div class="text-center">
                                    <button class="ms_btn ms_btn-grey" type="submit">Lean More</button>
                                </div>
                            </div>
                            

                        </div>

                    </div>

                </div>

            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MyCourses',
}
</script>

<style lang="scss" scoped>
@import "../../style/variables.scss";

.course{
    background-image: url(../../assets/promise-background.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    background-position:bottom;
}
    .box{
        background-color: $primaryColorCourses;
        box-shadow: 1px 8px 10px #cdd1cd;
        border-radius: 12px;
        overflow: hidden;

        .new-img{
            width: 50px;
            position: absolute;
            top: 0;
            left: 0;

        }

        p{
            color: $tertiaryColorCourses;
        }
    }

    .img-box{
        
        img{
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
    }

    .ms_text-color{
        color: $secondaryColorCourses;
    }
</style>