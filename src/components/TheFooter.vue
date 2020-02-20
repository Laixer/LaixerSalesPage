<template>
  <div class="footer">
    <div class="logo">
      <img src="@/assets/SVGlogo.svg" alt />
    </div>

    <div class="media">
      <a href class="linkedin">
        <img src="@/assets/SVGLinkedin.svg" alt />
        <p>LinkedIn</p>
      </a>
      <a href="https://github.com/laixer" class="github">
        <img src="@/assets/SVGGithub.svg" alt />
        <p>GitHub</p>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "theFooter"
};
</script>

<style lang="scss" scoped>
.footer {
  background: #022836;
  border: 1px solid #666f8f;
  opacity: 0.8;
  display: flex;
  padding: 25px;
  justify-content: space-between;
  flex-wrap: wrap;
}
.media {
  color: #a3a8bb;
  display: flex;
}
.logo {
}

.linkedin,
.github {
  padding: 10px;
  display: flex;
  justify-content: center;
  color: #a3a8bb;
  text-decoration: none;
  &:hover {
    color: lighten($color: #a4a8bb, $amount: 20%);
  }
}
p {
  padding: 7px;
}
@media screen and (max-width: 800px) {
  .footer {
    justify-content: center;
  }
  .logo {
    flex-basis: 100%;
    align-content: center;
    justify-content: center;
    display: flex;
    margin: 10px;
  }
}
</style>