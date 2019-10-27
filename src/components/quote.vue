<template>
    <div class="col-sm-4">
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
        border:1px solid #ccc;
        margin: 10px 0px;
        font-family: Arial, Helvetica, sans-serif
     }
    .quote{
        cursor: pointer
    }
    .quote:hover{
       background: rgb(255, 190, 190)
    }
</style>