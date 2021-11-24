<template>
    <div :class="city.rainyDays ? 'blue': 'yellow' ">
        <h2>{{city.name}}</h2>
        <article>
            <section>
                <h4> {{city.weekday1}} </h4>
                <h4> {{city.Sunday}}</h4>
            </section>

            <section>
                <h4>{{city.weekday2}} </h4>
                <h4> {{city.Monday}}</h4>
            </section>

            <section>
                <h4>{{city.weekday3}} </h4>
                <h4> {{city.Tuesday}}</h4>
            </section>

            <section>
                <h4>{{city.weekday4}} </h4>
                <h4> {{city.Wednesday}}</h4>
            </section>

            <section>
                <h4>{{city.weekday5}} </h4>
                <h4> {{city.Thursday}}</h4>
            </section>

            <section>
                <h4>{{city.weekday6}} </h4>
                <h4> {{city.Friday}}</h4>
            </section>

            <section>
                <h4>{{city.weekday7}} </h4>
                <h4> {{city.Saturday}}</h4>
            </section>
        </article>
    </div>

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
    background-color: #ffb89e;
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
}

article{
    display: flex;
    justify-content: center;
}


</style>