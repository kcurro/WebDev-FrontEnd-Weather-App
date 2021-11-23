<template>
<div class="container">
  <Header city="Southbury" state="CT"/>
  <About/>
</div>

  <!--<HelloWorld msg="Weclome to Class"/>-->
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'

import Header from './components/Header.vue'


//data url http://localhost:5555/books 
export default {
  name: 'App',
  components: {
    //HelloWorld
    Header
  },
}
</script>


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
  max-width: 400px;
  margin: 30px auto;
  overflow: auto;
  min-height: 300px;
  border: 0.3em solid black;
  padding: 30px;
  border-radius: 5px;
}

div{
  margin-bottom: 0.5em;
}
</style>
