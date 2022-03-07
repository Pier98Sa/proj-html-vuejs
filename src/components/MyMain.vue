<template>
    <main>
        <FormSection />
        <MyCTA />
        <MyCourses />
        <MySeparator />
        <MyStatistics />
        <MyInstructors />

    </main>
</template>


<script>
import FormSection from './partials/FormSection.vue'
import MyCTA from './partials/MyCTA.vue'
import MyCourses from './partials/MyCourses.vue'
import MySeparator from './partials/MySeparator.vue'
import MyStatistics from './partials/MyStatistics.vue'
import MyInstructors from './partials/MyInstructors.vue'

export default {
    name:'MyMain',
    components:{
        FormSection,
        MyCTA,
        MyCourses,
        MySeparator,
        MyStatistics,
        MyInstructors
    }

}
</script>

<style lang="scss" scoped>

    main{
        height: 1500px;
    }

</style>