<template>
  <nav class="navbar navbar-expand-lg fixed-top">
    <a class="navbar-brand" href="#"
      ><img src="@/assets/images/faymlogo.png" width="100" height="100" alt=""
    /></a>
    <button
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target="#navbarNav"
      aria-controls="navbarNav"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>
    <div id="navbarNav" class="collapse navbar-collapse">
      <ul class="navbar-nav ml-auto">
        <li class="nav-item active">
          <a class="nav-link" href="#">DISCOGRAPHY</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">VIDEOS</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">EVENTS</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">BLOG</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">SHOP</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#"><i class="ion-drag"></i></a>
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.navbar {
  background: #0d0405;
  .navbar-nav {
    margin: 10px 0px;
    .nav-item {
      .nav-link {
        color: #fff;
        font-size: 36px;
        font-family: 'Oswald', sans-serif;
        margin: 0px 10px;
      }
    }
  }
}
</style>
