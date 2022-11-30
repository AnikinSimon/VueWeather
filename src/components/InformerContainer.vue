<template>
    <div class="informer-container">
        <TemperatureShow :temperature-feel="temperatureFeel" :temperature-real="temperatureReal"/> 
        <div class="flex-break"></div>
        <HumidityShow :humidity="humidity"/> 
        <div class="vertical-divider"></div>
        <WindShow :wind="wind"/> 
    </div>
</template>

<script>
    import TemperatureShow from './TemperatureShow.vue'
    import HumidityShow from './HumidityShow.vue'
    import WindShow from './WindShow.vue'

    export default{
        name: 'InformerContainer',
        components: {
            TemperatureShow,
            HumidityShow,
            WindShow
        },
        data() {
            return {
                temperatureReal: 1,
                temperatureFeel: '-3.2',
                humidity: 6,
                wind: 20
            }
        }
    }
</script>

<style>
    .informer-container {
        display: flex;
        align-items: flex-start;
        justify-content: space-between;
        flex-wrap: wrap;
        width: 400px;
        min-height: 255px;
        padding: 30px;
        background-image: url('../assets/forest.png');
        background-size: cover;
        background-position: center center;
        border-radius: 20px;
        box-shadow: 0px 0px 10px 0px rgba(50, 50, 50, 0.75);
    }
    .flex-break{
        flex-basis: 100%;
        height: 0;
    }
    .vertical-divider{
        height: 70px;
        width: 1px;
        background-color: #fff;
        vertical-align: middle;
        display: table-cell;
    }
</style>
