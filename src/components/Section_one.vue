<template>
    <div class="section-one">
        <div class="group-one">
            <div class="title">
                LOREM <span class="color-highlight">IPSUM</span>
            </div>
            <div class="detail">
                <div class="d-one">Lorem Ipsum is simply Lorem Ipsum is simply Lorem Ipsum is simply</div><br>
                <div class="d-two">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's </div>
            </div>
        </div>
        <div class="group-two">
            <img :src="img_bicycle" alt="bicycle">
        </div>
    </div>
</template>

<script>
export default {
  data() {
    return {
      img_bicycle: '/imgs/Bicycle-PNG-Image 1.png'
    }
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Kanit&family=Montserrat:ital,wght@0,300;0,400;0,500;0,700;1,400;1,700&display=swap');
.section-one .title {
    color: white;
    position: absolute;
    width: 552px;
    height: 234px;
    left: 312px;
    top: 328px;

    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 700;
    font-size: 96px;
    line-height: 117px;
    text-transform: uppercase;
    color: #FFFFFF;

    text-shadow: 0px 4px 30px #21612F;
}
.group-one .detail {
    position: absolute;
    width: 440px;
    height: 52px;
    left: 312px;
    top: 631px;

    font-family: 'Montserrat';
    font-style: normal;
}
.group-one .d-one {
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    line-height: 24px;
    color: #FFFFFF;
}
.group-one .d-two {
    font-weight: 300;
    font-size: 18px;
    line-height: 150%;
    color: #FFFFFF;
}
.group-two {
    position: absolute;
    width: 858px;
    height: 504px;
    left: 817px;
    top: 328px;
}
</style>
