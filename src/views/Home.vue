<template>
  <div class="container">
      <div class="landing-section">
      <header class="landing-header">
        <div class="landing_name">
        <h2>Young Man's</h2>
        <h2>Madrassa</h2>
        <button class="btn ">LEARN MORE</button>
        </div>
        
          <!-- <h3>Compiled by</h3>
        <div class="compilers">
        <a href="https://github.com/androidm16" target="_blank">Siyabonga Mkhosana</a> <span class="splitLine" style="color: white">|</span>  <a href="https://github.com/Mogamat-Muneeb" target="_blank">Mogamat Muneeb Davids</a> <span class="splitLine" style="color: white">|</span>  <a href="https://github.com/Mullins69" target="_blank">Abdul-Atheem Mullins</a>
        </div> -->
      </header>
  </div>
  <div class="row">
    <div class="col who_we_are">
      <h1>Who we are</h1>
      <p>
       Young Man's Madrassa's vision is to produce well balanced, enlightened, empowered, independent-thinking, conscientious human beings, subscribing to Divine guidance and emulating the ideals of prophetic examples that play's a constructive role as compassionate and well informed individuals in society.
       Young Man's Madrassa was founded in 2018, and is located in , Manenberg Cape Town, South Africa. It was founded under the leadership of the Madrassa Tul Sadaqat. 
      </p>
    </div>
    <div class="col">
    <div class="overview">
      <div class="overview_section">
      <h1>Madrassa Overview</h1>
       <div class="overview_information">
          <div class="info">
            <h4>students</h4>

          </div>
          <div class="info">
            <h4></h4>

          </div>
          <div class="info">
            <h4></h4>

          </div>
          <div class="info">
            <h4></h4>

          </div>
       </div>
      </div>
    </div>
    </div>
  </div>
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'

export default {
  name: 'Home',
  components: {
    HelloWorld
  }
}
</script>

<style scoped>
.landing-section {
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  /* min-height: 50vh; */
  margin: 0;
  padding: 0;
  background-image: url("https://i.postimg.cc/DmV0mbGS/IMG-20220326-WA0097edit.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  /* margin-top: 70px; */
}
.landing-header {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  width: 100%;
  min-height: 100vh;
  background: rgba(0, 0, 0, 50%);
}
.landing_name h2 {
  font-size: 70px;
  font-weight: 600;
  color: #fff;
}
.landing_name {
  margin-top: -100px;
  margin-right:40%;
}
/* .landing-header h3 {
  font-size: 18px;
  font-weight: 700;
  color: #fff;
  padding-top: 70px;
} */
.landing-header h4 {
  color: #fff;
}
.who_we_are{
  margin-top:70px;
  text-align: left;
  margin-left: 20px;
  width: 50%;
}
.who_we_are p{
  margin-top: 20px;
  line-height: 25px;
}
.who_we_are h1{
  font-size: 30px;
  font-weight: 700;
  color:#047c46 ;
}



.overview {
  width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 50vh;
  /* margin: 0;
  padding: 0; */
  margin-top:60px ;
  background-image: url("https://i.postimg.cc/DmV0mbGS/IMG-20220326-WA0097edit.jpg");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  /* margin-top: 70px; */
}

.overview_section{
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  width: 100%;
  min-height: 50vh;
  background: rgba(0, 0, 0, 50%);
}

.overview_information{
  display: flex;
  justify-content: center !important; 
}

.info{
  display: flex;
  border: 3px solid;
  
  margin: 20%
}
@media only screen and (max-width: 770px) {
  .landing-header {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    width: 100%;
    flex-wrap: wrap;
    min-height: 80vh;
    background: rgba(0, 0, 0, 60%);
  }
  .landing-header h2 {
    font-size: 40px;
    font-weight: 700;
    color: #fff;
  }
  .landing-header h4 {
    color: #fff;
  }
  
}
</style>
