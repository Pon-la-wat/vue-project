<template>
    <div class="section-two">
        <div class="group-tree">
            LOREM IPSUM <span class="color-highlight">LOREM</span>
        </div>
        <div class="group-four">
            <img :src="img_ellipse" alt="ellipse">
        </div>
        <button class="btn-arrow-l"><font-awesome-icon :icon="['fas', 'fa-arrow-left']" class="icon alt"/></button>
        <button class="btn-arrow-r"><font-awesome-icon :icon="['fas', 'fa-arrow-right']" class="icon alt"/></button>
        <div class="detail">
            <div class="d-one">Lorem Ipsum is simply</div><br>
            <div class="d-two">Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
                when an unknown printer took a galley of type and scrambled it to make a type specimen book.
            </div>
        </div>
    </div>
</template>

<script>
export default {
  data() {
    return {
    //   img_ellipse: '/imgs/Ellipse 10.png'
      img_ellipse : new URL('/imgs/Ellipse 10.png', import.meta.url).href
    }
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Kanit&family=Montserrat:ital,wght@0,300;0,400;0,500;0,700;1,400;1,700&display=swap');
.section-two {
    position: absolute;
    width: 100%;
    height: 900px;
    left: 0px;
    top: 1018px;
}
.group-tree {
    position: absolute;
    left: 19.69%;
    right: 19.69%;
    top: 11.56%;
    bottom: 80.33%;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 700;
    font-size: 60px;
    line-height: 73px;
    text-align: center;
    text-transform: uppercase;
    color: #FFFFFF;
}
.group-four {
    position: absolute;
    left: 44.79%;
    right: 44.79%;
    top: 31.22%;
    bottom: 46.56%;
}
.btn-arrow-l {
    position: absolute;
    left: 0%;
    right: 97.14%;
    top: 47%;
    bottom: 46.89%;
}
.btn-arrow-r {
    position: absolute;
    left: 97.14%;
    right: 0%;
    top: 47%;
    bottom: 46.89%;
    background-color: #D9EF0C;
}
.section-two .detail .d-one {
    position: absolute;
    left: 42.14%;
    right: 42.08%;
    top: 60.22%;
    bottom: 36.22%;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 500;
    font-size: 26px;
    line-height: 32px;
    text-align: center;
    color: #FFFFFF;
    height: 32px;
    width: 303px;
}
.section-two .detail .d-two {
    position: absolute;
    left: 27.71%;
    right: 27.71%;
    top: 66%;
    bottom: 25%;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    line-height: 150%;
    text-align: center;
    color: #FFFFFF;
    height: 81px;
    width: 856px;
}
</style>
