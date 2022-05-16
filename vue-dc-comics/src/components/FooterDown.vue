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
                    <li><a href="#"><img src="../assets/img/footer-facebook.png" alt="#"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-twitter.png" alt="#"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-youtube.png" alt="#"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-pinterest.png" alt="#"></a></li>
                    <li><a href="#"><img src="../assets/img/footer-periscope.png" alt="#"></a></li>
                </ul>
            </div>
        </div>
    </footer>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import '../assets/style/vars';
@import '../assets/style/mixin';
footer{
    background-color: rgb(48, 48, 48);
    height: 100px;
    .container{
        @include row-centered;
        justify-content: space-between;
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
        @include row-centered;
        li{
            margin: 0 20px;
        }
    }
}

</style>