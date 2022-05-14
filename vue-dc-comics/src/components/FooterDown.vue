<template>
    <footer>
        <div class="container">
            <div class="sx">
                <a href="#">SIGN-UP NOW!</a>
            </div>
            <div class="dx">
                <ul class="follow-us">
                    <li>
                        <h4>
                            FOLLOW US
                        </h4>
                    </li>
                    <li :key="`social$${i}`" v-for="(el, i) in arraySocial">
                        <a :href="el.href">
                            <i :class="`fa-solid ${el.iconType} `"></i>
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    data(){
        return {
            arraySocial:[
                {
                    href: "#",
                    iconType: "fa-facebook"
                },
                {
                    href: "#",
                    iconType: "fa-twitter"
                },
                {
                    href: "#",
                    iconType: "fa-youtube"
                },
                {
                    href: "#",
                    iconType: "fa-patreon"
                },
                {
                    href: "#",
                    iconType: "fa-location-dot"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars';
footer{
    background-color: rgb(48, 48, 48);
    height: 100px;
    .container{
        display: flex;
        justify-content: space-between;
        align-items: center;
}
}
.sx{
    a{
        color: white;
        padding: 10px;
        border: 2px solid $dc-color;
    }
}
.dx{
    h4{
        color: $dc-color;
    }
    ul{
        display: flex;
        align-items: center;
        li{
            margin: 0 20px;
        }
    }
    i{
        font-size: 25px;
    }
}

</style>