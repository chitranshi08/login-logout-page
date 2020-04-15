<template>
  <div id="app">
  
    <LoginPage :login="login" v-if="!showDashboard"/>
    <Dashboard :userList="userList" :logout="logout" v-if="showDashboard"/>
  </div>
</template>

<script>
import LoginPage from './components/LoginPage.vue'
import Dashboard from './components/Dashboard.vue'
export default {
  name: 'App',
  components: {
    LoginPage,
    Dashboard
  },
  data:()=>({
    showDashboard:false,
    
  }),
  methods:{
    login(){
      this.showDashboard = true
    },
    logout(){
      this.showDashboard = false
    },
    


  }

}
</script>

<style>
@import "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.css";
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
body{
  background-color: #6d90f9;
  margin: 0;
  
  
}
</style>
