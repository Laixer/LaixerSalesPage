<template>
  <div class="index">
    <div class="mobile">
      <div class="container">
        <navbar></navbar>
        <hero></hero>
        <info></info>
        <!-- <textInfo></textInfo> -->
        <!-- <icons></icons> -->
        <aboutMe></aboutMe>
      </div>
      <theFooter></theFooter>
    </div>
    <div class="desktop">
      <div class="container">
        <navbar></navbar>
        <hero></hero>
        <info></info>
        <!-- <textInfo></textInfo> -->
        <!-- <icons></icons> -->
        <aboutMe></aboutMe>
      </div>
      <theFooter></theFooter>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

import navbar from '@/components/TheNavbar.vue';
import hero from '@/components/TheHero.vue';
import info from '@/components/InfoItems.vue';
import textInfo from '@/components/InfoText.vue';
import icons from '@/components/IconInfo.vue';
import aboutMe from '@/components/TheAbout.vue';
import theFooter from '@/components/TheFooter.vue';

@Component({
  name: 'home',
  components: {
    navbar,
    hero,
    info,
    textInfo,
    icons,
    aboutMe,
    theFooter,
  },
})
export default class Home extends Vue { }
</script>

<style lang="scss" scoped>
// .index {
// // background-color: #022836;
//   background-image: url("../assets/SVGBackground-mobile.svg");
//   background-size: cover;
//   display: block;
//     @media screen and (max-width: 800px) {
//       background-image: require("../assets/SVGBackground-mobile.svg");
//     }
// }

.container {
  max-width: 85%;
  margin: auto;
  @media screen and (max-width: 800px) {
    max-width: 90%;
  }
}
.desktop {
  background-image: url("~@/assets/images/SVGBackground.svg");
  background-size: cover;
  display: block;
}
.mobile {
  background-image: url("~@/assets/images/SVGBackground-mobile.svg");
  background-size: cover;
  display: none;
}
@media screen and (max-width: 800px) {
  .mobile {
    display: block;
  }
  .desktop {
    display: none;
  }
}
</style>
