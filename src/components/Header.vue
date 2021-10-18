<template>
  <h2>Dinmana Mana saja</h2>
  <h3>{{text}}</h3>
  <button @click="changeText">Ganti Text AJA</button>
</template>


<script>
export default {
  name:"Header",
 props:["text"],
 data(){
   return{
     newText : "Ini Text Bagian Baru"
   }
 },
 methods:{
   changeText(){
     this.$emit("changeTitle",this.newText);
   }
 },
 emits:["changeTitle"]
}
</script>

<style>

</style>
