<template>
     <div class="citybox">
         
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
}
</style>