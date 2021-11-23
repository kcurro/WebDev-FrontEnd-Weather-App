<template>
<div>
        <h4> {{site}} </h4>
        <h4> {{apiLink}} </h4>
</div>
</template>

<script>

export default{
    name: 'Reference',
    props:{
        site: String,
        apiLink: String
    }
}

</script>

<style scoped>

div{
    text-align: center;
}


</style>