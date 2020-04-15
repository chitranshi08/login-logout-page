<template>
  <div>
 	<div class="mainContainer">
      <div class="container">
    <h2>Login Page</h2>

 		<input type="text" class="emailInput" placeholder="Email-address"><br>
 		<input type="text" class="passwordInput" placeholder="Password"><br>

 		<button @click="login">login</button>
  </div>
  </div>
 	</div>

</template>

<script>
export default {
  name:'LoginPage',
  props:{
  	login:Function
  },
  data:()=>({

  }),
  	

  	
  
  methods:{
  	toggle:function(){
  		if(this.component === LoginPage){
  			this.component = Dashboard
  		}
  		else{
  			this.component = LoginPage
  		}

  	}
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>



.mainContainer{
 display: flex;
 justify-content:center;
 align-items: center;
 margin:auto;
 height:100vh;
 width:100vw;
 text-align: center;


}
.emailInput,.passwordInput{
  width:400px;
  margin-bottom: 15px;
  height: 35px;
  padding-left:10px;
  
}
button{
  background-color:blue;
  color:white;
  border: none;
  width:408px;
  height:40px;
  font-weight:bold;
  font-size:17px;
  cursor:pointer;

}
h2{
  color: white;
}




</style>
