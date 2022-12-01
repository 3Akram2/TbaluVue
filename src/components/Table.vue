<template>
    <v-table >
      <thead>
        <tr>
          <th class="text-left cell">
            Image
          </th>
          <th class="text-left cell">
            Select
          </th>
          <th class="text-left cell" >
            Actions
          </th>
        </tr>
      </thead>
      <tbody>
        <tr
          v-for="entry in entries"
          :key="entry.id"
        >
          <td> <img :src='entry.image' class="image" /> </td>
          <td> 
            <DropList  />
          </td>
          <td> <ButtonTwo text="delete" color="red" />
            <ButtonTwo text="edit" color="blue" />
        </td>

        </tr>
      </tbody>
    </v-table>
  </template>
  <script>
  import Image from "./Image.vue"
  import Button from './Button.vue';
import ButtonTwo from './ButtonTwo.vue';
  
import DropList from './DropList.vue';

  
  export default {
    components: {Button,
    DropList,
ButtonTwo,
Image,},
props:{
        entries:Array,
    },
    data() {
        return {
            
        };
    },
    components: { DropList, ButtonTwo, Image }
}
</script>
<style>
.image{
  height: 200px;
  width: 200px;
  border: 1px solid;
  margin: 1.5rem;
}
.cell{
  width: 30%;
}
</style>