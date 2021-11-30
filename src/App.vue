<template>
<div class="container">
  <Header title="Weekly Weather On The Go"
    subtitle="For the 6 Largest Cities in the U.S."/>
  <Reference site="Data sourced from Weather API "
   apiLink="openweathermap" />
  <Citybox :cities="cities" />
  <Contact msg1="Contact Our Developers"
    msg2="Thanks for visting the site!"/>
</div>

  <!--<HelloWorld msg="Weclome to Class"/>-->
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'

import Header from './components/Header.vue'
import Contact from './components/Contact.vue'
import Reference from './components/Reference.vue'
import Citybox from './components/Citybox.vue'

//data url https://intense-retreat-38934.herokuapp.com/api
export default {
  name: 'App',
  components: {
    Header,
    Reference,
    Citybox,
    Contact
  },

  data(){
      return {
        cities: []
      }
    },
    methods: {
       //promises

      async fetchCities(){
        const res= await fetch('https://intense-retreat-38934.herokuapp.com/api')
        console.log(res);
        const data= await res.json();
        console.log(data);
        return data;
      }
    },

    async created(){
      this.cities = await this.fetchCities();
    }
}
</script>

<!---app following color pallete https://coolors.co/cb997e-ddbea9-ffe8d6-b7b7a4-a5a58d-6b705c -->
<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300&display=swap');
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: 'Montserrat', sans-serif;
}
.container {
  display: grid;
  grid-gap: 0.5rem;
  border: 0.3em solid black;
  padding: 30px;
  border-radius: 5px;
  background-color: #FFE8D6;
}

div{
  margin-bottom: 0.5em;
}

</style>
