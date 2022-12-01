<template>
<v-tr>
          <td> {{entry.image}}</td>
          <td> 
            <DropList />
          </td>
          <td>   <ButtonTwo text="delete" color="red" />     </td>

        </v-tr>
</template>
<script>
import ButtonTwo from './ButtonTwo.vue';
import DropList from './DropList.vue';

import DropList from './DropList.vue';
export default{
    name: "Entry",
    props:{
        entry:Object,
    },
    components:{
    ButtonTwo,
    DropList,
    DropList
}
    ,
    methods:{
        onDelete(id){
            this.$emit('delete-entry',id)
        }
    }
}
</script>