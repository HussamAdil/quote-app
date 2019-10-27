<template>
    <div class="row">
        <form>
            <textarea v-model="quote"></textarea>
            <input type="submit" @click.prevent="CreateNewQuote" value="Add New Quote">
        </form>
     </div>
</template>
<script>
 
export default {
  data:function()
  {
      return {
          quote:'',
      }
  },
  methods:{
      CreateNewQuote()
      {
          if(this.quote === '')
          {
              return alert('empty sorry ')
          }
          this.$emit('NewquoteAdded' , this.quote)
          this.quote = ''
      }
  }
}
</script>
<style scoped>

</style>