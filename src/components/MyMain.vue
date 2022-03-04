<template>
    <main>
        <FormSection />
        <MyCTA />

    </main>
</template>


<script>
import FormSection from './partials/FormSection.vue'
import MyCTA from './partials/MyCTA.vue'

export default {
    name:'MyMain',
    components:{
        FormSection,
        MyCTA
    }

}
</script>

<style lang="scss" scoped>

    main{
        height: 1500px;
    }

</style>