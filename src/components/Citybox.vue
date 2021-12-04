<template>
     <div class="citybox">
        <div class = "index"> 
            <h4>Rain in the calendar: blue</h4>
            <h4>Sun in the calendar: yellow</h4>
        </div>


        <div v-for="city in cities" :key="city.id" >
                
                <City :city="city"/>
        </div>

        

     </div>

</template>

<script>

import City from "./City.vue"
export default{

    name: 'Citybox',
    components: {
        City
    },
    props: {
        cities: Array
    }

}

</script>


<style>

.citybox{

    background-color:#B7B7A4;
    padding: 1em;
    color: gray;

    /*display: inline-flex;
    flex-wrap: wrap;*/
    display: grid;
    justify-content: center;

}

.grid {
  display: grid;
  grid-template-columns: repeat(5, minmax(92px,1fr));
  gap: 10px;
}

.index{
    text-align: center;
    color: white;
}

</style>