<template>
 <VSelect
 @change="onItemSelcted"
  label="Select"
  :items="['California', 'Colorado', 'Florida', 'Georgia', 'Texas', 'Wyoming']"
  
></VSelect>

</template>


<script>
export default {
    
  data () {
    return {
      selectItem: 'Georgia',
      items: [
          'Georgia',
          'Florida',
         'Nebraska',
         'California',
         'New York' ,
      ],
    }
    
},
methods:{
  onItemSelcted()
    {
      console.log("===============================>")
    }
}  ,


}

</script>
<style>
.drop{
    margin: 5px;
}
</style>

