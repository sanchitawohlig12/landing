
<template>
  <div>
    <div class="container">
      <img
        class="img1"
        src="https://image.shutterstock.com/image-photo/abstract-splashes-water-on-black-600w-181096040.jpg"
        alt="Snow"
        style="width: 100%"
      />
      <div class="bottom-left"></div>
      <div class="top-left"></div>
      <div class="top-right"></div>
      <div class="bottom-right"></div>
      <div class="centered">
        <h1>Ultimate Platform to monitor your best workflow.</h1>
        <p>
          It should be noted that although application software is thought of as
          a program, it can be anything that runs on a computer.
        </p>
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

        <!--v-btn
          class="ma-2"
          src="https://www.youtube.com/embed/tgbNymZ7vqY"
          color="pink"
          dark
        >
          watch Our video
          <v-icon dark right> mdi mdi-message-video </v-icon>
        </!--v-btn!-->
      </div>
    </div>
  </div>
</template>
<style scoped>
.container {
  position: relative;
  text-align: center;
  color: white;
}

/* Bottom left text */
.bottom-left {
  position: absolute;
  bottom: 8px;
  left: 16px;
}

/* Top left text */
.top-left {
  position: absolute;
  top: 8px;
  left: 16px;
}

/* Top right text */
.top-right {
  position: absolute;
  top: 8px;
  right: 16px;
}

/* Bottom right text */
.bottom-right {
  position: absolute;
  bottom: 8px;
  right: 16px;
}

/* Centered text */
.centered {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
h1 {
  font-size: 40px;
}
.btn:hover {
  background-color: rgb(212, 39, 68);
  color: white;
}
.btn {
  background-color: white;
  color: black;
}
.img1 {
  height: 1000px;
}
</style>