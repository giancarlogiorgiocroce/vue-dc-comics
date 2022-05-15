<template>
  <footer>
    <div class="container">
      <div class="sx">
        <div class="col">
          <!-- DC Comics -->
          <ul>
            <li>
              <h3>DC COMICS</h3>
            </li>
            <li><a href="#">Characters</a></li>
            <li><a href="#">Comics</a></li>
            <li><a href="#">Movies</a></li>
            <li><a href="#">TV</a></li>
            <li><a href="#">Games</a></li>
            <li><a href="#">Video</a></li>
            <li><a href="#">News</a></li>
          </ul>
          <!-- Shop -->
          <ul>
            <li>
              <h3>SHOP</h3>
            </li>
            <li><a href="#">Shop DC</a></li>
            <li><a href="#">Shop DC Collectibles</a></li>
          </ul>
        </div>
        <div class="col">
          <!-- DC -->
          <ul>
            <li>
              <h3>DC</h3>
            </li>
            <li><a href="#">Terms of use</a></li>
            <li><a href="#">Privacy policy (New)</a></li>
            <li><a href="#">Ad Choises</a></li>
            <li><a href="#">Advertising</a></li>
            <li><a href="#">Jobx</a></li>
            <li><a href="#">Subscriptions</a></li>
            <li><a href="#">Talent Workshops</a></li>
            <li><a href="#">CPSC Certificates</a></li>
            <li><a href="#">Ratings</a></li>
            <li><a href="#">Shop Help</a></li>
            <li><a href="#">Contact Us</a></li>
          </ul>
        </div>
        <div class="col">
          <!-- Sites -->
          <ul>
            <li>
              <h3>SITES</h3>
            </li>
            <li><a href="#">DC</a></li>
            <li><a href="#">MAD Magazine</a></li>
            <li><a href="#">DC Kids</a></li>
            <li><a href="#">DC Universe</a></li>
            <li><a href="#">DC Power Visa</a></li>
          </ul>
        </div>
      </div>
      <div class="dx">
        <img src="../assets/img/dc-logo-bg.png" alt="Logo DC">
      </div>
    </div>
  </footer>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
footer{
    height: 400px;
    background-image: url(../assets/img/footer-bg.jpg);
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat; 
    overflow: hidden;

}
.container{
  display: flex;
  align-items: center;
}
.sx{
  display: flex;
  .col{
  width: 33%;
  }
  ul{
  color: white;
  height: 1;
  }
  li{
    margin-bottom: 10px;
  }
  h3{
    margin-bottom: 15px;
    margin-top: 20px;
  }
}
.sx,
.dx{
  width: 50%;
}
img{
  width: 100%;
}
</style>