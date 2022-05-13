<template>
  <section>
      <div class="container">
          <ul>
              <li :key="`shop${i}`" v-for="(el, i) in items">
                    <i :class="`fa-solid ${el.iconType}`"></i>
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
                    iconType: "fa-tablet-screen-button",
                },
                {
                    whatIsIt: "dc merchandise",
                    href: "#",
                    iconType: "fa-shirt",
                },
                {
                    whatIsIt: "subscriptions",
                    href: "#",
                    iconType: "fa-bolt",
                },
                {
                    whatIsIt: "comic shop locator",
                    href: "#",
                    iconType: "fa-location-dot",
                },
                {
                    whatIsIt: "dc power visa",
                    href: "#",
                    iconType: "fa-credit-card",
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars';
    section{
        height: 200px;
        background-color: $dc-color;
        color: white;
    }
    ul{
        height: 100%;
        display: flex;
        align-items: center;
        justify-content: space-around;
        li{
            display: flex;
            align-items: center;
        }
        i{
            font-size: 40px;
            margin: 0 20px;
        }
        a{
            text-transform: uppercase;
            color: white;
            font-size: 11px;
        }
    }
</style>