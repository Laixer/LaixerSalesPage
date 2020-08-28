<template>
  <div class="hero">
    <div class="text">
      <h1 class="title">
        The best way to predict the future is to create it.
        <span class="dot">.</span>
      </h1>
      <p>
        In the upcoming decade, every company will become a <span class="highlight">software company</span>.
        Take the <span class="highlight">lead</span>, don't follow.
        <!-- <span class="highlight">gravida</span> leo tempor id placerat erat, -->
        <!-- <span class="highlight">quis</span> rutrum libero. Aliquam erat volutpat. ac nulla Proin feugiat risus quis tristique blandit. -->
      </p>
      <button class="cta" onclick="location.href='mailto:info@laixer.com';">Get In Touch</button>
    </div>
  </div>
</template>

<script>
import { Component, Vue } from 'vue-property-decorator'

@Component({
  name: 'hero'
})
export default class TheHero extends Vue {}
</script>

<style lang="scss" scoped>
.text {
  margin-top: 50px;

  .title {
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
  }

  .highlight {
    color: #ffffff;
    text-decoration: underline double #3da8aa;
  }
  .dot {
    color: #7ed9da;
  }
  .cta {
    background: #022836;
    color: white;
    font-family: Montserrat;
    border: 2px solid #7ed9da;
    font-size: 20px;
    padding: 10px 20px;
    margin: 18px 0;
  }
}
@media screen and (min-width: 901px) {
  .text {
    margin-left: calc(50%);
    max-width: 40vw;
    margin-top: 200px;
  }
  p {
    text-align: center !important;
  }
  .cta {
    display: none !important;
  }
  .title {
    font-size: 4.2em !important;
    max-width: 100%;
  }
}
@media screen and (max-width: 450px) {
}
</style>
