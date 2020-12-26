<template>
  <form v-on:submit.prevent="onSubmit">
    <div>
      <label for="username">id : </label>
      <input type="text" id="username" v-model="username">
    </div>
    <div>
      <label for="password">password : </label>
      <input type="password" id="password" v-model="password">
    </div>
    <button type="submit" >login Button</button>
  </form>
</template>

<script>
import axios from 'axios';

export default {
  data: function(){
    return {
      username: '',
      password: ''
    }
  },
  methods:{
    onChange: function(){
      console.log('onChange clicked');
    },
    onSubmit: function(){
      console.log('submit clicked');
      console.log(this.username, this.password);
      var url = 'https://jsonplaceholder.typicode.com/users';
      var data = {
        username: this.username,
        password: this.password
      }
      axios.post(url,data).then(function(response){
        console.log(response);
      }).catch(function(error){
        console.log(error)
      });
    }
  }
}
</script>

<style>

</style>