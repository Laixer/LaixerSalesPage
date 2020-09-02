<template>
  <div class="about">
    <h1>
      About us
      <span class="dot">.</span>
    </h1>
    <p>
      We focus on internal development of ideas and products under our own management.
      <span
        class="highlight"
      >Developments</span> and
      <span class="highlight">Innovations</span>
      are directly applied and assessed where possible.
      In addition to our introvert-oriented culture, we support software development projects of partners.
    </p>

    <button class="button" onclick="location.href='mailto:info@laixer.com';">Get In Touch</button>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component({
  name: 'aboutMe',
})
export default class TheAbout extends Vue { }</script>

<style lang="scss" scoped>
.about {
  margin: 10vh 0;
}
h1 {
  text-transform: uppercase;
  font-family: "amsipro-black", sans-serif;
  color: #fff;
  font-size: 3.6em;
  margin-bottom: 10px;
  max-width: 80%;
}
p {
  font-size: 1.2em;
  font-family: "amsipro-regular", sans-serif;
  text-align: left;
  color: #ffffff;
  padding: 10px;
  background: #0000003b;
  max-width: 30%;
}
.highlight {
  color: #ffffff;
  text-decoration: underline double #3da8aa;
}
.dot {
  color: #7ed9da;
}
.button {
  margin: 20px 0px;

  background: #022836;
  color: white;
  font-family: Montserrat;
  border: 2px solid #7ed9da;
  font-size: 20px;
  padding: 10px 20px;
}
@media screen and (max-width: 900px) {
  p {
    max-width: 80%;
  }
}
</style>
