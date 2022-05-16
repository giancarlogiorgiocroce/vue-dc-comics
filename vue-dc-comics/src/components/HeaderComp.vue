<template>
  <header class="container">
      <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="DC logo">
      </div>
      <nav>
          <ul>
              <li v-for="(el, i) in navbar" :key="`navbar${i}`"
                :class="{'active': el.isActive}"
                @click="el.isActive = !el.isActive">
                  <a :href="el.href">{{el.name}}</a>
              </li>
          </ul>
      </nav>
  </header>
</template>

<script>
export default {
    data () {
      return {
        navbar:[
            {
                name: "characters",
                href: "#",
                isActive: false,
            },
            {
                name: "comics",
                href: "#",
                isActive: false,
            },
            {
                name: "movies",
                href: "#",
                isActive: true,
            },
            {
                name: "tv",
                href: "#",
                isActive: false,
            },
            {
                name: "games",
                href: "#",
                isActive: false,
            },
            {
                name: "collectibles",
                href: "#",
                isActive: false,
            },
            {
                name: "videos",
                href: "#",
                isActive: false,
            },
            {
                name: "fans",
                href: "#",
                isActive: false,
            },
            {
                name: "news",
                href: "#",
                isActive: false,
            },
            {
                name: "shop",
                href: "#",
                isActive: false,
            },
        ],
      }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars';
@import '../assets/style/mixin';
    header{
        @include row-centered;
        justify-content: space-around;
        height: 100px;
        border-bottom: 4px solid white;

        img{
            height: 75px;
        };
    }
    ul{
        @include row-centered;
        justify-content: space-between;
        li {
            padding: 40px 0;
            margin: 0 15px;
            border-bottom: 5px solid white;
            &.active{
                border-bottom: 5px solid $dc-color;
            }
            &.active a{
                color: $dc-color;
            }
        }
        a {
            text-transform: uppercase;
            font-size: 12px;
            font-weight: bold;
            &:hover{
                color: $dc-color;
            }
        }
    }
</style>