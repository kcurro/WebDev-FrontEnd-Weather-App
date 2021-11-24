<template>
    <div :class="city.rainyDays ? 'red': 'green' ">
                <h2>{{city.name}}</h2>
                        <article>

                <section>
                <h4> {{city.date1}}</h4>

        <h4> {{city.Sunday}}</h4>
                    </section>

        <section>
        <h4> {{city.date2}}</h4>

        <h4> {{city.Monday}}</h4>
                    </section>

        <section>
        <h4> {{city.date3}}</h4>


        <h4> {{city.Tuesday}}</h4>
                </section>

        <section>
        <h4> {{city.date4}}</h4>

        <h4> {{city.Wednesday}}</h4>
                </section>

        <section>
        <h4> {{city.date5}}</h4>

        <h4> {{city.Thursday}}</h4>
                </section>

        <section>
        <h4> {{city.date6}}</h4>

        <h4> {{city.Friday}}</h4>
                </section>

        <section>
        <h4> {{city.date7}}</h4>

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

.red{
background-color: orangered !important;

}

.green{
    background-color: green;
}

section{
    display: flex;
    justify-content: center;
}

article{
    display: flex;
    justify-content: center;
}


</style>