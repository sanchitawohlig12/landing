<template>
  <div class="banner-parallax-wrap" v-if="loaded">
    <v-row>
    <parallax :speed-factor="0.2" direction="down">
      <!--svg width="100px" height="100px" class="parallax-vertical parallax-dot">
        <use xlink:href="/images/decoration/dot-deco.svg#dot" />
      </!--svg!-->
    </parallax>

    <parallax :speed-factor="0.25" direction="down">
      <!--svg
        width="100px"
        height="100px"
        class="parallax-vertical parallax-triangle"
      >
        <use xlink:href="/images/decoration/triangle-deco.svg#triangle" />
      </!--svg!-->
    </parallax>

    <parallax :speed-factor="0.2" direction="down">
      <svg
        width="100px"
        height="100px"
        class="parallax-vertical parallax-circle"
      >
        <use xlink:href="/images/decoration/circle-deco.svg#circle" />
      </svg>
    </parallax>
  </div>
</template>

<style scoped lang="scss">
@import './feature-styles';
</style>

<script>
import Parallax from 'vue-parallaxy'
export default {
  components: {
    Parallax,
  },
  data: () => ({
    loaded: false,
  }),
  mounted() {
    this.loaded = true
  },
}
</script>
