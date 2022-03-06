<template>
    <main>
        <FormSection />
        <MyCTA />
        <MyCourses />
        <MySeparator />
        <MyStatistics />

    </main>
</template>


<script>
import FormSection from './partials/FormSection.vue'
import MyCTA from './partials/MyCTA.vue'
import MyCourses from './partials/MyCourses.vue'
import MySeparator from './partials/MySeparator.vue'
import MyStatistics from './partials/MyStatistics.vue'

export default {
    name:'MyMain',
    components:{
        FormSection,
        MyCTA,
        MyCourses,
        MySeparator,
        MyStatistics
    }

}
</script>

<style lang="scss" scoped>

    main{
        height: 1500px;
    }

</style>