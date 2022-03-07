<template>
<div class="Instructors mt-5">
    <div class="container-xl">
      <div class="row align-items-center">
          <div class="col-9">
              <h2 class="fs-1">Your Instructors</h2>
              <p class="fs-4 pt-4 my_p-color">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc ultrices auctor sapien id cursus. Aliquam maximus turpis in vehicula semper.</p>
          </div>

          <div class="col-3">
              <button type="submit" class="ms_btn ms_btn-green w-100">More about us</button>
          </div>
      </div>

      <div class="row mt-5">
          <div class="col-4" v-for="(instructor,index) in instructors" :key="index">
              <InstructorsCard :instructor='instructor'/> 
          </div>


      </div>
  </div>
</div>
  
</template>

<script>
import InstructorsCard from './InstructorsCard.vue'
export default {
    name: 'MyInstructors',
    components:{
        InstructorsCard
    },
    props:{
        instructors: Array
    }
}
</script>

<style lang="scss" scoped>
@import "../../style/variables.scss";
    .Instructors{
        background-color: $secondaryColorInstr;
        
        .my_p-color{
            color:$primaryColorInstr;
        }

        
    }

</style>