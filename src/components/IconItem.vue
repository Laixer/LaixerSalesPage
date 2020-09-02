<template>
  <div class="IconItems">
    <div class="item" v-for="dataitem in dataitems" v-bind:key="dataitem.id">
      <img src="@/assets/images/SVGSpeach.svg" alt class="icon" />
      <p>{{ dataitem.text }}</p>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';

@Component({
  name: 'iconInfo',
})
export default class IconItem extends Vue {
  private dataitems: Array<{ id: string, text: string }> = [
    {
      id: '1',
      text: 'Mauris a laoreet sem. Nam turpis purus, ',
    },
    {
      id: '2',
      text: 'Mauris a laoreet sem. Nam turpis purus, ',
    },
    {
      id: '3',
      text: 'Mauris a laoreet sem. Nam turpis purus, ',
    },
    {
      id: '4',
      text: 'Mauris a laoreet sem. Nam turpis purus, ',
    },
  ]
}
</script>

<style lang="scss" scoped>
.IconItems {
  display: flex;

  flex-wrap: wrap;
  justify-content: center;
}
.item {
  margin: auto;
  padding: 15px 0;

  img {
    margin-left: 15%;

    max-width: 40%;
  }

  p {
    color: #666f8f;
    align-self: auto;
    text-align: center;
    max-width: 70%;
    margin-top: 25px;
  }
}
@media screen and (max-width: 800px) {
  .item {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    margin: 18px 0px;
  }
  img {
    flex-basis: 100%;
    margin-left: 0% !important;
  }
  p {
    max-width: 40%;
  }
}
</style>
