<template>
        
<div class="progress">
	<div class="progress-bar" role="progressbar" aria-valuenow="60" aria-valuemin="0" aria-valuemax="100"
    :style="{width:(coutQuote / maxQuotes) * 100 + '%'}">
        {{maxQuotes}} / {{coutQuote}}
	</div>
</div>	

</template>
<script>
export default {
    props :['maxQuotes' , 'coutQuote']

}
</script>

<style scoped>

</style>