<template>
  <v-app>
    
    <NavBar/>
    
    <v-div class="bgImage">
    <div style="margin: 50px 50px 50px 50px">
      <v-row
      no-gutters
      style="height: 100px"
      align="center"
      justify="center"
      >
        <img class="mr-3" :src="require('./assets/gass.png')" height="90"/>
      <h1 class="fontAlter font-weight-black">Geo Africa Science Society</h1>
      </v-row>
    </div>
    
    <v-row
    style="width: 100%; margin-bottom: 30px"
    justify="center"
    align="center"
    no-gutters>
    <v-sheet
    class="centerSheet"
    color="rgba(1,1,1,0.5)"
    width="100%"
    height="35px"
    >
    <div style="width: 80%; margin:0 auto"><p class="text-subtitle-1" style="color: white"><marquee> STAY AT HOME. SAVE LIVES. HELP STOP THE CORONAVIRUS. <i class="fas fa-clinic-medical"></i></marquee></p></div>
    </v-sheet>
    </v-row>

    <div class="centerCarousel">
    <v-carousel
    class="rounded-lg"
    cycle
    height="400"
    hide-delimiter-background
    show-arrows-on-hover
  >
    <v-carousel-item
      v-for="item in items"
      :key="item.body"
      :src="item.url"
    >
        <v-row
        class="center"
          align="center"
          justify="center"
          no-gutters
        >
          <div style="width: 80%"> <p class="text-subtitle-1">{{ item.body }}</p></div>
        </v-row>
      <!-- <v-sheet
        height="100%"
      >
        
      </v-sheet> -->
    </v-carousel-item>
  </v-carousel>
  </div>
  </v-div>

  <Footer/>
  </v-app>
</template>

<script>
import NavBar from './components/NavBar.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    NavBar,
    Footer
  },
  data() {
    return {
      items:[
        {
          body:"Because of the COVID-19 Pandemic Situation, the planned Africa Oil & Power 2020 has been rescheduled to 5-7 October 2021 and will be held in Cape Town (South Africa).",
          url:"https://cdn.pixabay.com/photo/2020/04/03/19/02/virus-4999857_960_720.png"
        },
        {
          body:"The Solar Africa Exhibition scheduled to take place in Tanzania (Dar El Salem) from March 24 to 26, 2021.",
          url:"https://images.pexels.com/photos/861339/pexels-photo-861339.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940"
        },
        {
          body:"The 03rd Edition of Power & Energy Africa will take place in Ethiopia / Adis Ababa from 23-25 September, 2021.",
          url:"https://raw.githubusercontent.com/RyadAb/AffirmailyAssets/master/Annotation%202020-07-21%20161047.png"
        },
      ],
    }
  },

}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.center{
  background-color:rgba(1,1,1,0.5);
  margin: 0;
  width: 105%;
  height: 80px;
  position: absolute;
  top: 80%;
  left: 50%;
  -ms-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
}

.centerCarousel{
    width: 80%;
    margin: 0 auto;
    margin-bottom: 100px;
}

.fontAlter{
  font-family: Verdana, Geneva, Tahoma, sans-serif;
  
}

.bgImage{
  background-image: url('https://images7.alphacoders.com/893/893758.jpg');
  background-size: cover;
}

</style>
