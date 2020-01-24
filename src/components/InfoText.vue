<template>
  <div class="infoText">
      <div class="text">
          <p>Maecenas efficitur, ex vel maximus sollicitudin, tortor urna aliquam erat, in dictum nisl arcu iaculis ligula. Pellentesque ex eros, imperdiet in venenatis sit amet, gravida ullamcorper mauris.</p>
      </div>
  </div>
</template>

<script>
export default {
    name: "textInfo"

}
</script>

<style lang="scss" scoped>
.infoText{
    margin: 60vh 0;
    }
    

    .text {
        color: #7ED9DA;
        max-width: 50%;
        text-align: center;
        margin: auto;
        font-size: 1.2em;
        }
        
 @media screen and (max-width: 900px) {
     .text {
         max-width: 100%;
     }
 }
</style>