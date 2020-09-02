<template>
  <div class="info">
    <div class="item">
      <div class="text-box">
        <h2>Data Science & Machine learning</h2>
        <p>
          The technology of machine learning applied in data science are
          reaching a nexus of capability. This field of expertise is growing
          up fast and is limitless. Our mindset is that you can have data
          without information, but you cannot have information without data.
          Torture the data, and it will confess to anything.
        </p>
      </div>
    </div>
    <div class="item reverse">
      <div class="img-box"></div>
      <div class="text-box">
        <h2>COMPUTER SCIENCE & QUALITY BY DESIGN</h2>
        <p>
          Digital product engineering can only be as good as its design.
          Subsequently a foundation can only be made with a multidisciplinary
          set of capabilities and knowledge. Computer Science is a science of
          abstraction, creating the right model for any set of problems and
          devising the appropriate mechanizable techniques to solve it. We
          combine proven principles with newly developed technology to bring
          customers competitive edge in their marketplaces. We can assist in
          problem solving and design innovative systems.
        </p>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component({
  name: 'info',
})
export default class InfoItems extends Vue { }
</script>

<style lang="scss" scoped>
.info {
  display: flex;

  flex-wrap: wrap;

  .item {
    margin-top: 10vh;
    display: flex;
    flex-wrap: wrap;
  }
  .text-box {
    margin: 40px;
    width: 50%;
    float: right;
    h2 {
      text-align: left;
      text-transform: uppercase;
      font-family: "amsipro-black", sans-serif;
      src: url("~@/assets/fonts/AmsiPro-Black.otf");
      font-size: 3.6em;
      color: #ffffff;
      margin-bottom: 2vw;
    }
    p {
      padding: 20px;
      background: #0000003b;
      font-size: 1.5vw;
      font-family: "amsipro-regular", sans-serif;
      src: url("~@/assets/fonts/AmsiPro-Regular.ttf");
      text-align: left;
      color: #ffffff;
    }
  }
  .img-box {
    width: 40%;
  }
}
@media screen and (max-width: 900px) {
  .text-box {
    width: 100% !important;
  }
  .img-box {
    width: 100% !important;
  }
  .reverse {
    flex-wrap: wrap-reverse !important;
  }
  h2 {
    font-size: 3.1em !important;
    text-align: center !important;
  }
  p {
    font-size: 3vw !important;
    text-align: center !important;
  }
}
</style>
