<template>
  <div class="container-fluid">
    <section class="landing-page-wrapper">
      <AppMusicPlayerComponent />
    </section>
    <section class="latest-section">
      <div class="row">
        <div class="col-6 text-center">
          <h3>LATEST SINGLE</h3>
          <hr class="horizonal-line hr-1" />
          <div class="song-details-wrapper">
            <img src="@/assets/images/songimage.png" alt="" />
            <h4 class="track-name">TEST ME</h4>
          </div>
        </div>
        <div class="col-6 text-center">
          <h3 class="text-center">OFFICIAL VIDEO</h3>
          <hr class="horizonal-line hr-2" />
          <div class="video-wrap">
            <div class="video">
              <iframe
                width="693"
                height="536"
                src="https://www.youtube.com/embed/0pThnRneDjw"
                frameborder="0"
                gesture="media"
                allowfullscreen
              ></iframe>
            </div>
            <a href="" class="">VIEW MORE VIDEOS</a>
          </div>
        </div>
      </div>
    </section>
    <section class="parallax"></section>
    <section class="releases">
      <div class="">
        <h3 class="text-center">MORE RELEASES</h3>
        <hr />
        <div class="container-fluid">
          <div class="row text-center">
            <div class="col-md-4">
              <img
                src="@/assets/images/freematter.png"
                class="img-fluid"
                alt=""
              />
              <p class="">FREE MATTER</p>
            </div>
            <div class="col-md-4">
              <img
                src="@/assets/images/makeitofficial.png"
                class="img-fluid"
                alt=""
              />
              <p class="">MAKE IT OFFICIAL</p>
            </div>
            <div class="col-md-4">
              <img
                src="@/assets/images/nobeplay.png"
                class="img-fluid"
                alt=""
              />
              <p>NO BE PLAY</p>
            </div>
          </div>
          <div class="row">
            <a href="" class="text-center mx-auto">VIEW MORE RELEASES</a>
          </div>
        </div>
      </div>
    </section>
    <section class="parallax2"></section>
    <section class="gallary">
      <div class="">
        <h3 class="text-center">PORTOFOLIOS</h3>
        <hr />
        <div class="container-fluid">
          <div class="row">
            <div class="col-md-4">
              <img src="@/assets/images/faym4.png" class="img-fluid" alt="" />
            </div>
            <div class="col-md-4">
              <img src="@/assets/images/faym5.png" class="img-fluid" alt="" />
            </div>
            <div class="col-md-4">
              <img src="@/assets/images/faym6.png" class="img-fluid" alt="" />
            </div>
          </div>
          <div class="row">
            <a href="" class="text-center mx-auto">VIEW MORE PORTFOLIOS</a>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import AppMusicPlayerComponent from '@/components/AppMusicPlayerComponent.vue'
export default {
  components: {
    AppMusicPlayerComponent,
  },
}
</script>

<style lang="scss" scoped>
.landing-page-wrapper {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.latest-section {
  margin: 50px 0px;
  h3 {
    font-family: 'Oswald', sans-serif;
    font-style: normal;
    font-weight: 500;
    font-size: 89.3113px;
    line-height: 132px;
    color: #ffffff;
  }
  .horizonal-line {
    background: #fff;
    padding: 3px;
    border-radius: 10%;
    width: 40%;
    margin: auto;
  }
  .song-details-wrapper {
    margin: 55px 0px;
    img {
      width: 693px;
      height: 536px;
    }
    .track-name {
      font-family: Oswald;
      font-style: normal;
      font-weight: 700;
      font-size: 65px;
      line-height: 115px;
      color: #ffffff;
    }
  }
  .video-wrap {
    margin: 55px 0px;
    a {
      font-family: 'Oswald', sans-serif;
      font-style: normal;
      font-size: 36px;
      line-height: 55px;
      color: #ffffff;
      margin: 15px;
      border-bottom: 2px;
    }
  }
}
.parallax {
  /* The image used */
  background-image: url('../assets/images/faym.png');

  /* Full height */
  height: 100vh;
  /* Create the parallax scrolling effect */
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.parallax2 {
  /* The image used */
  background-image: url('../assets/images/faym2.png');

  /* Full height */
  height: 100vh;
  /* Create the parallax scrolling effect */
  background-attachment: fixed;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}
.releases {
  margin: 50px 0px;
  h3 {
    font-family: 'Oswald', sans-serif;
    font-style: normal;
    font-weight: 700;
    font-size: 89.3113px;
    line-height: 132px;
    color: #ffffff;
  }
  hr {
    padding: 2px;
    background-color: #fff;
    width: 25%;
    margin: 30px auto;
  }
  .container-fluid {
    margin-top: 40px;
  }
  img {
    width: 509px;
    height: 480px;
  }
  p {
    font-family: 'Oswald', sans-serif;
    font-style: normal;
    font-weight: 700;
    font-size: 50px;
    line-height: 132px;
    color: #fff;
  }
  a {
    font-family: 'Oswald', sans-serif;
    font-style: normal;
    font-weight: 400;
    font-size: 36.8181px;
    line-height: 55px;
    color: #ffffff;
  }
}
.gallary {
  margin: 50px 0px;
  h3 {
    font-family: 'Oswald', sans-serif;
    font-style: normal;
    font-weight: 700;
    font-size: 89.3113px;
    line-height: 132px;
    color: #ffffff;
  }
  hr {
    padding: 2px;
    background-color: #fff;
    width: 25%;
    margin: 30px auto;
  }
  .container-fluid {
    margin-top: 40px;
    margin-bottom: 40px;
  }
  img {
    width: 509px;
    height: 480px;
  }
  a {
    font-family: 'Oswald', sans-serif;
    font-style: normal;
    font-weight: 400;
    font-size: 36.8181px;
    line-height: 55px;
    color: #ffffff;
    margin: 50px 0px;
  }
}
</style>
