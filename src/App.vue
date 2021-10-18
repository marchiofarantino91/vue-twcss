<template>
<Header @changeTitle="ubahText" :text="text"/>
</template>
<script>

import Header from "./components/Header.vue"
export default {
  name: 'App',
  components:{
    Header
  },
  data(){
    return{
      text:"Selamat Datang dari Data!"
    }
  },
methods:{
  ubahText(newText){
    this.text = newText;
  }
}
}
</script>

<style>

</style>
