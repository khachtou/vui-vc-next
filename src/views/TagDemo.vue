<template>
  <div id="app">
    <router-link to="/" class="m-back">&lt; Home</router-link>
    <div class="m-example">
      <p>Tag Share - Circle</p>
      <v-tag type="fill" size="tiny" shape="circle" fill-color="#FC5353">100</v-tag>
      <v-tag type="fill" size="small" shape="circle" fill-color="#36C" font-color="#FFF">promotion</v-tag>
      <v-tag type="ghost" size="small" shape="circle">10%</v-tag>
      <v-tag
        type="fill"
        size="small"
        shape="circle"
        sharp="bottom-right"
        fill-color="#36C"
        font-color="#FFF"
      >half price</v-tag>
    </div>
    <div class="m-example">
      <p>Tag Shape - Special</p>
      <v-tag type="fill" shape="coupon" fill-color="#36C" font-color="#FFF">Coupon Ticket</v-tag>
      <v-tag type="fill" shape="quarter" fill-color="#FC9191" font-color="#FFF">&times;</v-tag>
      <v-tag type="fill" shape="bubble" font-color="#FFF">88</v-tag>
    </div>
    <div class="m-example">
      <p>Tag Shape - No fill color</p>
      <v-tag type="fill" shape="square" fill-color="rgba(0, 0, 0, 0)">&pound;100</v-tag>
    </div>
  </div>
</template>

<script>
import { defineComponent } from 'vue'
import VTag from '../components/tag/index.vue'

export default defineComponent({
  name: 'tag-demo',

  inheritAttrs: false,

  components: {
    VTag
  }
})
</script>

<style scoped>
.m-back {
  display: block;
  margin: 0.2rem;
  font-size: 0.3rem;
  text-decoration: none;
}

.m-example {
  margin: 0.2rem;
  padding-bottom: 0.4rem;
  font-size: 0.4rem;
  border-bottom: 1px solid #ccc;
}

.m-example p {
  padding-bottom: 0.2rem;
}

.m-example .m-tag {
  margin-right: 0.5rem;
}
</style>