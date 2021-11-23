<template>
<div>
    <h1> {{title}} </h1>
    <h4> {{subtitle}} </h4>
</div>
</template>

<script>

export default{
    name: 'Header',
    props:{
        title: String,
        subtitle: String
    }
}

</script>

<style scoped>

div{
    text-align: center;
    background-color: #ddbea9;
}

</style>