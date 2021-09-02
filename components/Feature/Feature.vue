<template>
  <div>
    <section id="main" class="space-top space-bottom">
      <main-feature />
    </section>
    <!--section id="parallax">
      <parallax-feature />
    </!--section!-->
    <section id="more">
      <more-feature />
    </section>
  </div>
</template>

<script>
//import Parallax from './Parallax'
import MainFeature from './MainFeature'
import MoreFeature from './MoreFeature'

export default {
  components: {
    //'parallax-feature': Parallax,
    MainFeature,
    MoreFeature,
  },
}
</script>
<style scoped lang="scss">
@function section-margin($margin) {
  @return $margin * 5;
}

.space-bottom {
  margin-bottom: section-margin($spacing1);
}
.space-top {
  padding-top: section-margin($spacing1);
}
</style>
