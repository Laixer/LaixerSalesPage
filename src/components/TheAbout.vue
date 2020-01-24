<template>
<div class="about">

    <h1>About us<span class="dot">.</span></h1>
    <p>Nam et arcu in metus aliquet porta. Vivamus lobortis <span class="highlight">molestie</span> pretium. Curabitur libero diam, sodales eget neque a, imperdiet facilisis purus. Praesent euismod dictum purus, non auctor quam auctor non. <br><br> Aliquam et eleifend quam. Sed scelerisque elit sed sem efficitur mattis.</p>

     <button class="button">
         Get In Touch
     </button> 
      
</div>
</template>

<script>
export default {    name: 'aboutMe'

}
</script>

<style lang="scss" scoped>

.about {
    margin:  50vh 0;
}
h1 {
            text-transform: uppercase;
        font-family: 'amsipro-black', sans-serif; 
        color: #fff;
        font-size: 3.6em;
        margin-bottom: 10px;
        max-width: 80%;
}
p {
            font-size: 1.2em;
        font-family: 'amsipro-regular-16', sans-serif;
        text-align: left;
        color: #666F8F; 
        max-width: 30%;
}
    .highlight {
        color: #FFFFFf;
        text-decoration: underline double #3DA8AA; 
    }
    .dot {
        color: #7ED9DA;
    }
    .button {
          margin: 20px 0px;

    background: #022836;
    color: white;
    font-family: Montserrat;
    border: 2px solid #7ED9DA;
    font-size: 20px;
    padding: 10px 20px;
  }
    @media screen and (max-width: 900px) {
        p {
            max-width: 80%;

        }

    }

</style>