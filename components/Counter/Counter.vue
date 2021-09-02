<template>
  <div class="counter-wrap">
    <div id="watched_counter" />
    <v-container>
      <v-row>
        <v-col sm="4" cols="12">
          <div class="counter-item">
            <div class="text" style="text-align: center">
              <h4 class="display-1" v-if="loaded">
                <span
                  v-countUp:onWindowScroll.once="{
                    watchedElId: 'watched_counter',
                    startValue: 0,
                    endValue: 123,
                    options: { duration: 1 },
                  }"
                />
              </h4>
              <h6 class="title">completed project</h6>
            </div>
          </div>
        </v-col>
        <v-col sm="4" cols="12">
          <div class="counter-item">
            <div class="text" style="text-align: center">
              <h4 class="display-1" v-if="loaded">
                <span
                  v-countUp:onWindowScroll.once="{
                    watchedElId: 'watched_counter',
                    startValue: 0,
                    endValue: 456,
                    options: { duration: 1 },
                  }"
                />
              </h4>
              <h6 class="title">Lines Code</h6>
            </div>
          </div>
        </v-col>
        <v-col sm="4" cols="12">
          <div class="counter-item">
            <div class="text" style="text-align: center">
              <h4 class="display-1" v-if="loaded">
                <span
                  v-countUp:onWindowScroll.once="{
                    watchedElId: 'watched_counter',
                    startValue: 0,
                    endValue: 789,
                    options: { duration: 1 },
                  }"
                />
              </h4>
              <h6 class="title">Team Members</h6>
            </div>
          </div>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<style scoped lang="scss">
@import './counter-style';
</style>

<script>
export default {
  data: () => ({
    loaded: false,
  }),
  mounted() {
    this.loaded = true
  },
}
</script>
