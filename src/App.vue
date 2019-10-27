<template>
    <div class="container">
        <apphead :maxQuotes="maxQuotes" :coutQuote="quotes.length"></apphead>
        <newQuote @NewquoteAdded="PushNewQuote"></newQuote>
    <quoteGrid :quotes="quotes" @quoteDeleted="deleteQuote"></quoteGrid>
    <div class="row">
        <div class="col-sm-12 text-center">
            <div class="alert alert-info">You can Delete Quote By click them</div>
        </div>
    </div>
    </div>
</template>

<script>
import newQuote from './components/NewQuote.vue'

import quoteGrid from './components/QuoteGrid.vue'

import apphead from './components/head.vue'

    export default {
        components:{quoteGrid:quoteGrid,newQuote:newQuote,apphead:apphead},
        data :function()
        {
           return {
               maxQuotes : 10,
                  quotes:  [ ' Just for testing ']
            }
        },
        methods:{
            PushNewQuote(quote)
            {
                if(this.quotes.length === 5 )
                {
                   return  alert('sorry first delete one ')
                }
                this.quotes.push(quote)
            },
            deleteQuote(index)
            {
                this.quotes.splice(index,1)
            }
        }
    }
</script>

<style>
</style>
