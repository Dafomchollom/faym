<template>
  <div class="music-player-wrapper stickty-bottom">
    <div class="audio-player">
      <div class="album-art-wrapper">
        <div class="image-wrapper">
          <img src="@/assets/images/albumArt.png" alt="" />
        </div>
        <div class="song-details">
          <p class="song-title">TEST ME</p>
          <p class="artist-name">FAYM OFFICIAL</p>
        </div>
      </div>
      <div class="play-buttons-wrapper">
        <button class="repeat">
          <i class="ion-ios-loop"></i>
        </button>
        <button class="prev">
          <i class="ion-ios-skipbackward"></i>
        </button>
        <button class="play"><i class="ion-play"></i></button>
        <button class="next"><i class="ion-ios-skipforward"></i></button>
        <button class="shuffle"><i class="ion-ios-shuffle"></i></button>
      </div>
      <div class=""></div>
      <!-- <div class="seek-bar">
        <div class="fill"></div>
        <div class="handle"></div>
      </div> -->
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
:root {
  background-color: #222;
}

$brown: #feecae;

.music-player-wrapper {
  position: absolute;
  width: 100%;
  bottom: 0%;
  .audio-player {
    display: flex;
    // flex-wrap: wrap;
    // justify-content: center;
    // align-items: center;
    background: #1d1d1d;
    .album-art-wrapper {
      width: 33.33%;
      text-align: left;
      display: flex;
      flex-wrap: wrap;
      // justify-content: center;
      align-items: center;
      .image-wrapper {
        width: 35%;
        img {
          width: 199px;
          height: 176px;
        }
      }
      .song-details {
        height: 100%;
        width: 65%;
        padding: 40px 0px;
        align-items: center !important;
        .song-title {
          font-family: 'Oswald', sans-serif;
          font-style: normal;
          font-weight: 700;
          font-size: 42.0723px;
          line-height: 50px;
          color: #ffffff;
          margin: 0px;
        }
        .artist-name {
          font-family: 'Oswald', sans-serif;
          font-style: normal;
          font-weight: 200;
          font-size: 30.0723px;
          // line-height: 62px;
          margin: 0px;
          color: #ffffff;
        }
      }
    }
    .play-buttons-wrapper {
      width: 33.33%;
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: center;
      button {
        display: block;
        border: 0;
        color: white;
        border-radius: 100000px;
        margin: 0px 15px;
        font-size: 27px;
        background: transparent;
      }
      button.play {
        width: 105px;
        height: 105px;
        background-color: $brown;
        color: #000;
        font-size: 50px;
        border-radius: 100000px;
        cursor: pointer;
      }
    }

    .seek-bar {
      margin: 30px;
      width: 400px;
      background-color: white;
      display: flex;
      align-items: center;
      border-radius: 100000px;
      cursor: pointer;

      .fill {
        height: 10px;
        background-color: $brown;
        border-radius: 100000px;
      }

      .handle {
        width: 10px;
        height: 10px;
        background-color: $brown;
        border-radius: 100000px;
        margin-left: -5px;
        transform: scale(2);
        transition: all 0.1s;

        &:hover {
          background-color: lighten($brown, 10%);
          transform: scale(3);
        }
      }
    }
  }
}
</style>
