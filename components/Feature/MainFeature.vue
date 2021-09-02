<template>
  <div>
    <h1>We always try to quality work</h1>
    <p>
      Quis ipsum suspendisse ultrices gravida. Risus commodo viverra maecenas
      accumsan lacus vel facilisis.
    </p>
    <v-row>
      <v-col>
        <v-hover>
          <template v-slot:default="{ hover }">
            <v-card class="mx-auto" max-width="344">
              <v-card-text>
                <h2 class="text-h6 primary--text">Modern Design</h2>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua. Quis
                ipsum suspendisse ultrices gravida.
              </v-card-text>
              <v-expand-transition>
                <v-overlay v-if="hover" absolute color="pink"> </v-overlay>
              </v-expand-transition>
            </v-card>
          </template>
        </v-hover>
      </v-col>
      <v-col>
        <v-hover>
          <template v-slot:default="{ hover }">
            <v-card class="mx-auto" max-width="344">
              <v-card-text>
                <h2 class="text-h6 primary--text">Modern Design</h2>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua. Quis
                ipsum suspendisse ultrices gravida.
              </v-card-text>
              <v-expand-transition>
                <v-overlay v-if="hover" absolute color="pink"> </v-overlay>
              </v-expand-transition>
            </v-card>
          </template>
        </v-hover>
      </v-col>
      <v-col>
        <v-hover>
          <template v-slot:default="{ hover }">
            <v-card class="mx-auto" max-width="344">
              <v-card-text>
                <h2 class="text-h6 primary--text">Modern Design</h2>
                Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
                eiusmod tempor incididunt ut labore et dolore magna aliqua. Quis
                ipsum suspendisse ultrices gravida.
              </v-card-text>
              <v-expand-transition>
                <v-overlay v-if="hover" absolute color="pink"> </v-overlay>
              </v-expand-transition>
            </v-card>
          </template>
        </v-hover>
      </v-col>
    </v-row>
  </div>
</template>
<style scoped>
h1 {
  text-align: center;
}
p {
  text-align: center;
}
</style>