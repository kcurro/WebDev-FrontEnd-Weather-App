<template>


</template>

<script>

import City from "./City.vue"
export default{

    name: 'Citybox',
    components: {
        City
    },
    props: {
        city: Array
    }

}

</script>


<style>

.citybox{

    background-color: bisque;
    padding: 1em;
    color: gray;
}
</style>