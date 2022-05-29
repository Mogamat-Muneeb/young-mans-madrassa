<template>
<Navbar />
<main>
  <router-view :key="$route.fullPath"/>
 </main>
 <!-- <Footer /> -->
</template>
<script>
import Navbar from "./components/Navbar.vue";
// import Footer from "./components/Footer.vue";
export default {
  components: { Navbar } 
  };
</script>
<style>

*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

#app {
  font-family: "Nunito",sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: rgb(41, 39, 39);

 
}

body{
   overflow-x: hidden;
  overflow-y:scroll;
  -ms-overflow-style: none;
  scrollbar-width: none;  
}
body::-webkit-scrollbar{
  display:none;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: rgb(41, 39, 39);
  text-decoration:none; 
  margin-top: -7px;
}

#nav a.router-link-exact-active {
  color: #047c46;
  text-decoration: none;
}

#nav a:hover{
  font-weight: bold;
  color:#047c46;
  text-decoration:none; 
  transition:0.5s
}


</style>
