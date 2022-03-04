<template>
    <main>
        <FormSection />

    </main>
</template>


<script>
import FormSection from './partials/FormSection.vue'

export default {
    name:'MyMain',
    components:{
        FormSection
    }

}
</script>

<style lang="scss" scoped>

    main{
        height: 1500px;
    }

</style>