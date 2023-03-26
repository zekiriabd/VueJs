
<script setup>
import UserList from './components/userList/UserList.vue'
</script>

<template>

<h1>App Page</h1>

<div class="card" style="width: 18rem;">
  <div class="card-body">
    <UserList :user="myuser" 
    @OnchngedUserName="OnchngedUserName($event)"/>
  </div>
</div>
</template>

<script>
export default{
  data() {
    return {
      myuser:"zekiri abdelali",
    }
  },
  methods:{
    OnchngedUserName(val){
      console.log("btn is clicked",val.name);      
    }
  }
 
}
</script>
<style scoped>
</style>
