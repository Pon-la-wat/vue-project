<template>
    <nav class="navbar">
        <ul class="nav">
            <li class="logo">
                <img :src="img_logo" alt="logo">
                <div class="logo-name">
                    LOREM <span class="color-highlight"> IPSUM</span>
                </div>
            </li>
            <li class="nav-item">
                <a href="#lorem">LOREM</a>
                <a href="#lorem" class="dropdown">LOREM <font-awesome-icon icon="fa-solid fa-chevron-down" /></a>
                <a href="#loremipsum">LOREMIPSUM</a>
                <a href="#lorem&ipsum">LOREM & IPSUM</a>
                <a href="#lorem">LOREM</a>
            </li>
        </ul>
    </nav>
</template>

<script>
export default {
  data() {
    return {
    //   img_logo: '/imgs/kindpng_546104 2.png'
      img_logo : new URL('/imgs/kindpng_546104 2.png', import.meta.url).href
    }
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Kanit&family=Montserrat:ital,wght@0,300;0,400;0,700;1,400;1,700&display=swap');
.navbar {
    position: relative;
    display: flex;
    width: 100%;
    height: 150px;
    justify-content: center;
    align-items: center;
    background: #000000;
    box-shadow: 0px 4px 25px rgba(0, 0, 0, 0.06);
}
.nav {
    position: absolute;
    width: 1573px;
    height: 100px;
    display: flex;
    align-items: center;
    padding-inline-start: 0px;
}
.logo {
    display: table;
    width: auto;
    height: 87px;
}
.logo-img {
    width: 74px;
    height: 87px;
}
.logo-name {
    display: table-cell;
    text-align: center;
    vertical-align: middle;
    padding-left: 10px;

    font-family: 'Montserrat';
    font-style: italic;
    font-weight: 700;
    font-size: 24px;
    line-height: 29px;
    text-transform: uppercase;
}
.nav-item {
    display: flex;
    flex-direction: row;
    align-items: flex-start;
    padding: 0px;
    gap: 30px;

    position: absolute;
    left: 23.5%;
    right: 41.2%;
    top: 39%;
    bottom: 39%;
}
.nav-item > a {
    color: white;
    text-decoration: none;

    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 300;
    font-size: 18px;
    line-height: 22px;

    flex: none;
    order: 0;
    flex-grow: 0;
}
.logo-img, .logo-name, .nav-item {
    list-style-type: none;
}
.dropdown {
    position: relative;
    margin-right: 18px;
}
.fa-chevron-down {
    position: absolute;
    font-size: 10px;
    top: 20%;
    left: 110%;
}
</style>
