<template>
  <div class="feature-more">
    <v-container>
      <u-animate-container>
        <scroll-wrap target="feature1">
          <v-row id="feature1">
            <v-col md="6" class="px-6" cols="12">
              <div class="feature-item">
                <u-animate name="" duration="0.6s">
                  <h3 class="title-app display-2">
                    Make your website more powerful
                  </h3>
                  z
                </u-animate>
                <u-animate name="" delay="0.3s" duration="0.6s">
                  <p class="text">
                    We Design & Develop Websites that stand out of the crowd.
                    Alea is an extremely feature rich, beautiful WordPress
                    Template.
                  </p>
                </u-animate>
                <u-animate-container>
                  <scroll-wrap target="feature1">
                    <v-row id="feature1">
                      <v-col md="6" class="px-6" cols="12">
                        <u-animate name="" duration="0.6s">
                          <v-btn class="ma-2" color="pink" dark>
                            Friendly Interface
                            <v-icon dark right> mdi-laptop </v-icon>
                          </v-btn>
                          <p>
                            Make your website more powerful Make your website
                            more powerful Make your website more powerful
                          </p>
                        </u-animate>
                        <u-animate name="" duration="0.6s">
                          <v-btn class="ma-2" color="pink" dark>
                            Powerfull Options
                            <v-icon dark right>
                              mdi-format-list-bulleted
                            </v-icon>
                          </v-btn>
                          <p>
                            Make your website more powerful Make your website
                            more powerful Make your website more powerful
                          </p>
                        </u-animate>
                      </v-col>
                      <v-col md="6" class="px-6" cols="12">
                        <div class="feature-item">
                          <u-animate name="zoomIn" delay="0.3s" duration="0.6s">
                            <div class="deco1" />
                          </u-animate>
                          <u-animate name="" duration="0.6s">
                            <v-btn class="ma-2" color="pink" dark>
                              Organize Code
                              <v-icon dark right>
                                mdi-format-align-bottom
                              </v-icon>
                            </v-btn>

                            <p>
                              Make your website more powerful Make your website
                              more powerful Make your website more powerful
                            </p>
                          </u-animate>
                          <u-animate name="" duration="0.6s">
                            <v-btn class="ma-2" color="pink" dark>
                              Premium Support
                              <v-icon dark right> mdi-music-box </v-icon>
                            </v-btn>

                            <p>
                              Make your website more powerful Make your website
                              more powerful Make your website more powerful
                            </p>
                          </u-animate>

                          <v-btn
                            class="
                              btn
                              mx-auto
                              lg:mx-0
                              gradient
                              text-white
                              font-bold
                              rounded-full
                              my-6
                              py-4
                              px-8
                              shadow-lg
                            "
                          >
                            Get Started
                          </v-btn>
                        </div>
                      </v-col>
                    </v-row>
                  </scroll-wrap>
                </u-animate-container>
              </div>
            </v-col>
            <v-col md="6" class="px-4" cols="12">
              <div class="feature-item">
                <u-animate name="zoomIn" delay="0.3s" duration="0.6s">
                  <div class="deco1" />
                </u-animate>
                <u-animate name="" delay="0.5s" duration="0.6s">
                  <figure class="img">
                    <img
                      class="img"
                      src="https://genial-react.envytheme.com/images/about-img1.jpg"
                      alt="img"
                    />
                  </figure>
                </u-animate>
              </div>
            </v-col>
          </v-row>
        </scroll-wrap>
      </u-animate-container>
    </v-container>
  </div>
</template>

<style scoped lang="scss">
@import './feature-styles';
.btn:hover {
  background-color: rgb(212, 39, 68);
  color: white;
}
.btn {
  background-color: white;
  color: black;
}
</style>

<script>
import ScrollWrap from '../ScrollWrap'
import imgAPI from '~/static/images/imgAPI'

export default {
  components: {
    ScrollWrap,
  },
  data() {
    return {
      imgAPI,
    }
  },
}
</script>
<style scoped>
.text {
  font-size: 5px;
}
.img {
  height: 400px;
  width: 2000px;
}
</style>


