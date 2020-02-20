<template>
  <div class="hero">
    <div class="text">
      <h1 class="title">
        Lorem ip sit amett sum dolor
        <span class="dot">.</span>
      </h1>
      <p>
        Morbi posuere sagittis lorem, non
        <span class="highlight">gravida</span> leo tempor id placerat erat,
        <span class="highlight">quis</span> rutrum libero. Aliquam erat volutpat. ac nulla Proin feugiat risus quis tristique blandit.
      </p>
      <button class="cta">Get In Touch</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "hero"
};
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
    font-family: "amsipro-regular-16", sans-serif;
    text-align: left;
    color: #666f8f;
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