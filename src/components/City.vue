<template>
    <article>

    <div :class="city.rainyDays ? 'blue': 'yellow' ">
        <h2>{{city.name}}</h2>
        <div class="cityinfo">
            <section>
                <h4> {{city.weekday1}} </h4>
                <h6> {{city.date1}}</h6>
                <h4> {{city.Sunday}}</h4>
            </section>

            <section>
                <h4>{{city.weekday2}} </h4>
                <h6> {{city.date2}}</h6>
                <h4> {{city.Monday}}</h4>
            </section>

            <section>
                <h4>{{city.weekday3}} </h4>
                <h6> {{city.date3}}</h6>
                <h4> {{city.Tuesday}}</h4>
            </section>

            <section>
                <h4>{{city.weekday4}} </h4>
                <h6> {{city.date4}}</h6>
                <h4> {{city.Wednesday}}</h4>
            </section>

            <section>
                <h4>{{city.weekday5}} </h4>
                <h6> {{city.date5}}</h6>
                <h4> {{city.Thursday}}</h4>
            </section>

            <section>
                <h4>{{city.weekday6}} </h4>
                <h6> {{city.date6}}</h6>
                <h4> {{city.Friday}}</h4>
            </section>

            <section>
                <h4>{{city.weekday7}} </h4>
                <h6> {{city.date7}}</h6>
                <h4> {{city.Saturday}}</h4>
            </section>
    </div>
</div>
</article>

</template>

<script>

export default{
    name: 'City',
    props:{
        city: Array
    }
}
</script>

<style scoped>



h4{
    margin: 2px;
}

div{
    color: black;
    padding: 1em;
}

.blue{
background-color:lightblue !important;

}

.yellow{
    background-color: lightgoldenrodyellow;
}

section{
    display: block;
    justify-content: center;
    font-size: 10;
    border-radius: 5px;
    padding: 10px;
    border: 0.1em solid black;
    color: darkslategray;
    text-align: center;

}

article{
    display: grid;
    /*display: grid;*/
    justify-content: center;
    /*border: 0.1em solid lightslategray;*/
    /*padding: 30px;*/
}

.cityinfo{

    display: inline-flex;
    flex-wrap: wrap;
    /*display: inline-grid;
    justify-content: center;*/
}


</style>