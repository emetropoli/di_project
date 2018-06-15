<template>
  <div>
    <img class="kiosco" src="~assets/kiosk2.png" />
    <Navigation />
    <nuxt/>
  </div>
</template>

<script>
import Navigation from '~components/Navigation.vue'

export default {
  components: {
    Navigation
  }
}
</script>

<style>
.kiosco {
  position: absolute;
  right: 0;
  top: 133px;
  width: 350px;
  z-index: 10;
}

@media screen and (max-width: 700px) {
  .kiosco {
    z-index: 0;
  }
}
</style>
