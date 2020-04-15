<template>
  <div>
   <div class="mainContainer">
     <span @click="logout" class="fa fa-power-off"></span>
   </div>
   <div class="container">
     <div class="sidenav"></div>
      <div class="contentPage"></div>
   </div>
   </div>
  
</template>

<script>
export default {
  name:'Dashboard',
  
  props:{
  	logout:Function,
    abcPage:Function,
  },
  data:()=>({
    
  }),
  

  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>


body{
  background-color: blue;
}
button{
	
}
.mainContainer{
  height: 60px;
  width:100vw;
  position:relative;
  background-color: black;
}
.container{
  display:flex;

}
.sidenav{
  height: 100vh;
  width: 200px;
  background-color: black;
}
.contentPage{
  width:calc(100% - 200px);
  background: white;
}
span{
color:white;
position:absolute;
top:20px;
right:50px;
font-size: 25px;
cursor: pointer;
}



</style>
