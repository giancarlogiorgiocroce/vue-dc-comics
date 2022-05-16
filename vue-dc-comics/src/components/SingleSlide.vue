<template>
  <div class="box">
      <div class="img">
          <img :src="comic.thumb" :alt="comic.series">
      </div>
      <h5>{{comic.series}}</h5>
  </div>
</template>

<script>

export default {
    props:{
        comic: Object,
    }
}
</script>

<style lang="scss" scoped>
.box{
    display: flex;
    align-items: flex-start;
    flex-direction: column;
    flex-basis: calc((100% / 6) - 20px);
    margin: 10px;

    .img{
        width: 21vh;
        height: 21vh;
        overflow: hidden;
        img{
            width: 100%;
        }
    };
}

h5{
    color: lightgrey;
    text-transform: uppercase;
    margin-top: 20px;
}

</style>