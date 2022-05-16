<template>
  <section>
      <div class="container">
          <ul>
              <li :key="`shop${i}`" v-for="(el, i) in items">
                    <img :src="el.src" :alt="el.whatIsIt">
                    <a :href="el.href">
                        {{el.whatIsIt}}
                    </a>
              </li>
          </ul>
      </div>
  </section>
</template>

<script>
export default {
    data(){
        return{
            items:[
                {
                    whatIsIt: "digital comics",
                    href: "#",
                    src: require('../assets/img/buy-comics-digital-comics.png')
                },
                {
                    whatIsIt: "dc merchandise",
                    href: "#",
                    src: require('../assets/img/buy-comics-merchandise.png'),
                },
                {
                    whatIsIt: "subscriptions",
                    href: "#",
                    src: require('../assets/img/buy-comics-subscriptions.png'),
                },
                {
                    whatIsIt: "comic shop locator",
                    href: "#",
                    src: require('../assets/img/buy-comics-shop-locator.png'),
                },
                {
                    whatIsIt: "dc power visa",
                    href: "#",
                    src: require('../assets/img/buy-dc-power-visa.svg'),
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars';
@import '../assets/style/mixin';
    section{
        height: 200px;
        background-color: $dc-color;
        color: white;
    }
    ul{
        height: 100%;
        @include row-centered;
        justify-content: space-around;
        li{
            @include row-centered;
            justify-content: center;
            min-width: 200px;
        }
        img{
            max-width: 50px;
            max-height: 50px;
            margin: 0 10px;
        }
        a{
            text-transform: uppercase;
            color: white;
            font-size: 11px;
        }
    }
</style>