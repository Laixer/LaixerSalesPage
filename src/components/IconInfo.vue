<template>
  <div class="icons">
    <h1>Lorem ipsum dolor amet, consectetur ?</h1>
    <div class="items">
      <iconInfo></iconInfo>
    </div>
  </div>
</template>

<script>
import iconInfo from "@/components/IconItem.vue";
export default {
  name: "icons",
  components: {
    iconInfo
  }
};
</script>

<style lang="scss" scoped>
h1 {
  margin: auto;
  text-align: center;
  font-size: 3.6em;
  color: white;
}
.items {
  margin: 15vh 0;
}
</style>