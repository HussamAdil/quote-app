<template>
    <div class="row">
       <quote v-for=" (quote , index) in quotes" @click.native="deleteQuote" :key="index">{{quote}}</quote> 
    </div>
</template>
<script>
    import  quote from './quote.vue'

export default {
    props:['quotes'],
    components:{quote:quote},
    methods:{
        deleteQuote(index)
        {
            this.$emit('quoteDeleted' , index)
        }
    }
}
</script>
<style scoped>

</style>