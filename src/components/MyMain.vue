<template>
    <main>
        <FormSection />
        <MyCTA />
        <MyCourses />

    </main>
</template>


<script>
import FormSection from './partials/FormSection.vue'
import MyCTA from './partials/MyCTA.vue'
import MyCourses from './partials/MyCourses.vue'

export default {
    name:'MyMain',
    components:{
        FormSection,
        MyCTA,
        MyCourses
    }

}
</script>

<style lang="scss" scoped>

    main{
        height: 1500px;
    }

</style>