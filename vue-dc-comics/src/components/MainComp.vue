<template>
  <main>
    <div class="current">CURRENT SERIES</div>

    <div class="container">

        <SingleSlide 
            :key="i"
            v-for="(el, i) in arrayComics"
            :comic="el"/>

    </div>

    <div class="btn">LOAD MORE</div>
  </main>
</template>

<script>
import SingleSlide from './SingleSlide.vue';
import dcComics from '../assets/data/dc-comics.json';

export default {
    components: { SingleSlide },
    data(){
        return{
            arrayComics: dcComics,
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars.scss';

main{
    background-color: black;
    padding: 50px 20px 20px 20px;
    color: white;
    position: relative;

    .current{
        background-color: $dc-color;
        padding: 15px 35px;
        display: inline;
        position: absolute;
        top: -20px;
        left: 150px;
    
    }

    .container{
        display: flex;
        flex-wrap: wrap;
    }

    .btn{
        background-color: $dc-color;
        width: 200px;
        text-align: center;
        line-height: 30px;
        margin: 0 auto;
    }
}

</style>