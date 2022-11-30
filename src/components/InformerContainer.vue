<template>
    <div class="informer-container">
        <TemperatureShow/> 
        <div class="flex-break"></div>
        <HumidityShow/> 
    </div>
</template>

<script>
    import TemperatureShow from './TemperatureShow.vue'
    import HumidityShow from './HumidityShow.vue'

    export default{
        name: 'InformerContainer',
        components: {
            TemperatureShow,
            HumidityShow
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
</style>
