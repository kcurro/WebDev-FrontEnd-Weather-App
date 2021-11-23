<template>
<div>
    <h1> {{city}} </h1>
    <h4> {{state}} </h4>
</div>
</template>

<script>

export default{
    name: 'Header',
    props:{
        city: String,
        state: String
    }
}

</script>

<style scoped>

div{
    text-align: center;
}

</style>