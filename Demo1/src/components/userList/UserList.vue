<template src="./UserList.html"/>
<style src="./UserList.css"></style>

<script>
export default{
  props:[
    'user'
  ],
  data() {
    return {
        name:"Zekiri abdelali",
    }
  },
  methods:{
    SetUsername(){
      this.name='Mohamed';
      this.$emit("OnchngedUserName",{name:"1111111111111"});
    }
  }
}
</script>