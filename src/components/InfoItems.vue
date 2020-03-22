<template>
  <div class="info">
    <div class="item">
      <div class="text-box">
        <h2>Data Science & Machine learning</h2>
        <p>The technology of machine learning applied in data science are reaching a nexus of capability. This field of expertise is growing up fast and is limitless. Our mindset is that you can have data without information, but you cannot have information without data. Torture the data, and it will confess to anything.</p>
      </div>

      <div class="img-box">
        <p>img here</p>
      </div>
    </div>
    <div class="item reverse">
      <div class="img-box">
        <p>img here</p>
      </div>
      <div class="text-box">
        <h2>COMPUTER SCIENCE & QUALITY BY DESIGN</h2>
        <p>Digital product engineering can only be as good as its design. Subsequently a foundation can only be made with a multidisciplinary set of capabilities and knowledge. Computer Science is a science of abstraction, creating the right model for any set of problems and devising the appropriate mechanizable techniques to solve it. We combine proven principles with newly developed technology to bring customers competitive edge in their marketplaces. We can assist in problem solving and design innovative systems.</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "info"
};
</script>

<style lang="scss" scoped>
.info {
  display: flex;

  flex-wrap: wrap;

  .item {
    margin-top: 70vh;
    display: flex;
    flex-wrap: wrap;
  }
  .text-box {
    margin: 40px;
    width: 50%;
    h2 {
      text-align: left;
      text-transform: uppercase;
      font-family: "amsipro-black", sans-serif;
      font-size: 3.6em;
      color: #ffffff;
      margin-bottom: 2vw;
    }
    p {
      font-size: 1.5vw;
      font-family: "amsipro-regular-16", sans-serif;
      text-align: left;
      color: #666f8f;
    }
  }
  .img-box {
    width: 40%;
    border: solid 1px white;
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
