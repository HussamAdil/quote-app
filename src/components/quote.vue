<template>
    <div class="col-4">
        <div class="panel-body quote">
            <slot></slot>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
    .panel-body
    {
        font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif
    }
    .quote{
        cursor: pointer
    }
    .quote:hover{
       background: rgb(197, 46, 46)
    }
</style>