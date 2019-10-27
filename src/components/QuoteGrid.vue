<template>
    <div class="row">
       <quote v-for="quote in quotes" :key="quote">{{quote}}</quote> 
    </div>
</template>
<script>
    import  quote from './quote.vue'

export default {
    props:['quotes'],
    components:{quote:quote}
}
</script>
<style scoped>

</style>