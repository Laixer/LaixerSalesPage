<template>
  <div id="app">
    <link
      href="https://fonts.googleapis.com/css?family=Montserrat&display=swap"
      rel="stylesheet"
    />
    <router-view />
  </div>
</template>

<style lang="scss">
@font-face {
  font-family: "amsipro-regular";
  src: url("~@/assets/fonts/AmsiPro-Regular.ttf");
  font-weight: normal;
  font-style: normal;
  font-display: swap;
}

@font-face {
  font-family: "amsipro-black", sans-serif;
  src: url('~@/assets/fonts/AmsiPro-Black.otf');
  font-weight: normal;
  font-style: normal;
  font-display: swap;
}

#app {
  font-family: "amsipro-regular", sans-serif;
}
* {
  padding: 0;
  margin: 0;
}
</style>
