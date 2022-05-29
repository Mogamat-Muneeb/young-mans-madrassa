<template>


<nav id="nav" class="links" :class="{ active: isActive}">
    <div class="container">
        <a class="navbar-brand" href="/">
              <!-- <img src="https://i.postimg.cc/0jT0TT91/download.png" alt=""> -->
        </a>   
    </div>
 
    <router-link @click="toggleNav" to="/">Home</router-link>
     <router-link @click="toggleNav" :to="{ name: 'About'}">About Us</router-link>
    <router-link @click="toggleNav" :to="{ name: 'What_we_do'}">What We Do</router-link>
    <router-link @click="toggleNav" :to="{ name: 'Gallery'}">Gallery</router-link>
    <router-link @click="toggleNav" :to="{ name: 'Contact'}">Contact Us</router-link>
</nav>    
<button id="nav-btn" @click="toggleNav">
    <i class="fa fa-bars"></i>
</button>    

</template>

<script>
export default {
    data(){
        return {
            isActive: false,
        };
    },
    methods:{
        toggleNav() {
            this.isActive = !this.isActive;
        },
    },
};
</script>

<style scoped>

.links{
    
    display:flex;
    justify-content:end;
    gap: 15px;      
}
#nav{
    z-index: 100;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 60px;
    background: white;
    /* box-shadow:8px 8px 15px #e4e4e4; */

    
}

#nav-btn{
    position: fixed;
    top: 10px;
    right: 30px;
    background: #f5f5f5;
    /* box-shadow:8px 8px 15px #e4e4e4; */
    padding: 10px;
    border-radius: 50%;
    height: 50px;
    width: 50px;
    border: none;
    outline: none;
    display: none;
    overflow-x: hidden;
}

.navbar-brand {
    position: fixed;
    left: 15px;
    top: 5.5px;
}

img{
    height:55px;
    width:55px;
}
@media screen and (max-width:700px) {
    #nav{
        position: fixed;
        height:100%;
        left: -200vw;
        display:flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        transition:left 0.7s linear;
        gap: 40px;
    }
    #nav.active{
        left:0;
    }
    #nav-btn{
        display:block;
        z-index: 100;
        

        
    }
 
}

.navbar-brand:hover{
  transform: translate(-3px, -3px);
   transition:1.5s
}
</style>