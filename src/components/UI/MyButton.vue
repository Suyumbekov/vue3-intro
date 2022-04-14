<template>
   <button class="btn">
        <slot></slot>
   </button>  
</template>

<script>
    export default {
        name: 'my-button'
    }
</script>

<style scoped>
.btn{
    background:none;
    color:teal;
    padding:10px 15px;
    border: 2px solid teal;
}
</style>
