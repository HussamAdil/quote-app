<template>
    <div class="container">
    <quoteGrid :quotes="quotes"></quoteGrid>
    </div>
</template>

<script>
import quoteGrid from './components/QuoteGrid.vue'
    export default {
        components:{quoteGrid:quoteGrid},
        data :function()
        {
           return {
               maxQuoutes : 10,
                  quotes:  [ ' Just for testing ']
            }
        }
    }
</script>

<style>
</style>
