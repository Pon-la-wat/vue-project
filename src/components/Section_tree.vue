<template>
    <div class="section-tree">
        <div class="group-five">
            LOREM IPSUM
        </div>
        <div class="group-six">
            <div class="card" v-for="product in products">
                <img v-bind:src="product.thumbnail" />
                <div class="card-body">
                    <br>
                    <div class="title">{{ product.title }}</div><br>
                    <div class="description">{{ product.description }}</div>
                    <!-- <div class="rating">rating</div>
                    <div class="price">${{ product.price }}</div> -->
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import axios from 'axios'

export default {
  data() {
    return {
        products: []
    }
  },
  created() {
    axios.get('https://dummyjson.com/products?limit=3')
      .then(response => {
        this.products = response.data.products;
      })
      .catch(error => {
        console.log(error);
      })
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Kanit&family=Montserrat:ital,wght@0,300;0,400;0,500;0,700;1,400;1,700&display=swap');
.section-tree {
    position: absolute;
    width: 100%;
    height: 900px;
    left: 0px;
    top: 1918px;
    background: #D9EF0C;
}
.group-five {
    position: absolute;
    height: 82px;
    left: 728px;
    top: 130px;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 700;
    font-size: 60px;
    line-height: 82px;
    text-align: center;
    letter-spacing: 0.02em;
    text-transform: capitalize;
    color: #000000;
}
.group-six {
    position: absolute;
    width: 1296px;
    height: 443px;
    left: 312px;
    top: 280px;
    /* filter: drop-shadow(0px 4px 40px rgba(0, 0, 0, 0.3)); */
    display: flex;
    flex-wrap: nowrap;
}
.card {
    position: relative;
    background-color: #f1f1f1;
    margin: 0 12px;
    height: 443px;
    width: 416px;
    border-radius: 4px;
}
.card:hover {
    transition-duration: 200ms;
    filter: drop-shadow(0px 5px 15px rgba(100, 107, 8, 0.5));
}
.card-body {
    /* border: 1px solid red; */
    position: absolute;
    padding: 25px;
    top: 48%;
    background-color: #f1f1f1;
    height: 170px;
}
.section-tree .title {
    padding: 0;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 500;
    font-size: 26px;
    color: #000000;
}
.section-tree .description {
    bottom: 15.8%;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 300;
    font-size: 18px;
    line-height: 130%;
    color: #333333;
}
.section-tree .price {
    position: absolute;
    bottom: 5%;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    line-height: 130%;
    color: red;
}
.section-tree .rating {
    position: absolute;
    bottom: 20%;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 400;
    font-size: 18px;
    line-height: 130%;
    color: red;
}
.section-tree .card img {
    position: absolute;
    top: 0%;
    bottom: 46.73%;
    max-width: 100%;
    height: auto;
    border-radius: 4px;
}
</style>
