<template>
  <div class="container-fluid">
    <div class="landing-page-wrapper">
      <AppMusicPlayerComponent />
    </div>
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

<style>
.landing-page-wrapper {
  margin: 0 auto;
  min-height: 190vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>
