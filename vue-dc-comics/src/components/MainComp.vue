<template>
  <main>
      <div class="container">
          <SingleSlide 
            :key="i"
            v-for="(el, i) in arrayComics"
            :comic="el"/>
      </div>
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
main{
    margin-top: 1.5px;
    background-color: black;

    .container{
        display: flex;
        flex-wrap: wrap;
    }

    h1{
        color: white;
        font-size: 30px;
        font-weight: bold;
    }
}

</style>