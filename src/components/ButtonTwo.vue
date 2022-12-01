<template>
    <v-btn class="btn"
  :color='color'
  elevation="11"
  large
  
  
> {{text}}</v-btn>
</template>
<script>
export default{
    props:{
        text:String,
        color:String,
    }
}

</script>
<style>
.btn{
    margin: 5px;
}
</style>
