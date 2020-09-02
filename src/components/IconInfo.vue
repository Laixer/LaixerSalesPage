<template>
  <div class="icons">
    <h1>Lorem ipsum dolor amet, consectetur ?</h1>
    <div class="items">
      <iconItem></iconItem>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import IconItem from '@/components/IconItem.vue';

@Component({
  name: 'icon',
  components: { IconItem },
})
export default class IconInfo extends Vue { }
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
