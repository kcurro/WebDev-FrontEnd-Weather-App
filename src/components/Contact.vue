<template>
<div>
    <h1> {{msg1}} </h1>
    <item>
        <h4><font-awesome-icon icon="envelope" /></h4>
        <a href="mailto: kcurr3@unh.newhaven.edu">   Email</a>
    </item>
    <h4> {{msg2}} </h4>
</div>
</template>

<script>

export default{
    name: 'Contact',
    props:{
        msg1: String,
        msg2: String
    }
}

</script>

<style scoped>

div{
    text-align: center;
    background-color: #ddbea9;

}

item{
    display: flex;
    justify-content: center;

}
</style>