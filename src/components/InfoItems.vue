<template>
  <div class="info">

<div class="item">
    <div class="text-box">
        <h2>Lorem ipsum, Dolor ametT?</h2>
        <p>Nam et arcu in metus aliquet porta. Vivamus lobortis molestie pretium. Curabitur libero diam, sodales eget neque a, imperdiet facilisis purus. Praesent euismod dictum purus, non auctor quam auctor non.</p>
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
        <h2>Integer nec nunc nec erat?</h2>
        <p>Vestibulum ut ultricies libero, vel sagittis elit. Ut sagittis arcu ipsum, quis suscipit ante aliquam non. Etiam tempus nisi ornare vestibulum lobortis. Proin a faucibus tellus. Suspendisse placerat id orci nec tincidunt. In egestas auctor risus, at placerat velit. Integer ullamcorper, est congue scelerisque congue, sapien lectus pulvinar velit, porta suscipit risus quam id purus. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia Curae; Morbi dapibus interdum justo. Nullam ut venenatis eros, in porta felis.</p>
    </div>
</div>




  </div>
</template>

<script>

export default {

    
    name: 'info',


}
</script>

<style lang="scss" scoped>

.info {
    display: flex;

      flex-wrap: wrap;
      
    .item{ 
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
            font-family: 'amsipro-black', sans-serif; 
            font-size: 3.6em;
            color: #ffffff;
            margin-bottom: 2vw;
        }
        p {
            font-size: 1.5vw;
            font-family: 'amsipro-regular-16', sans-serif;
            text-align: left;
            color: #666F8F;
        }
    }
    .img-box {
        width: 40%;
        border: solid 1px white;

        
    }
}
 @media screen and (max-width: 900px)  {
     .text-box {
         width: 100% !important;
 
     }
     .img-box {

         width: 100% !important;
     }
     .reverse{ 
         flex-wrap: wrap-reverse !important;
     }
     h2 {
font-size:  3.1em!important;
         text-align: center !important;   
     }
     p {
            font-size: 3vw !important;
                     text-align: center !important;   
     }
 }

</style>
