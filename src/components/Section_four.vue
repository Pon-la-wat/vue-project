<template>
    <div class="section-four">
        <img :src="img_bicycle" alt="bicycle">
        <div class="group-seven">
            <div class="contact-title">
                ติดต่อเรา
            </div>
            <div class="contact-body">
                <input type="text" class="form-control" placeholder="ชื่อ - นามสกุล">
                <input type="text" class="form-control" placeholder="เบอร์ติดต่อ">
                <input type="text" class="form-control" placeholder="อีเมล">
                <div class="form-calendar">
                    <input type="text" class="form-control" placeholder="วันที่">
                    <div onclick="alert('OK')">
                        <font-awesome-icon :icon="['fas', 'fa-calendar-days']" class="icon alt"/>
                    </div>
                </div>
                <div class="contact-detail">
                    Lorem ipsum dolor sit amet consectetur, adipisicing elit. Atque reprehenderit impedit tempora quam doloremque,
                    repudiandae corporis natus eligendi enim.
                </div>
                <button class="btn btn-success">LOREM</button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  data() {
    return { 
        img_bicycle : new URL('/imgs/Bicycle-PNG-Image 1.png', import.meta.url).href
    }
    // return {
    //   img_bicycle: '/imgs/Bicycle-PNG-Image 1.png'
    // }
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Kanit&family=Montserrat:ital,wght@0,300;0,400;0,500;0,700;1,400;1,700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Kanit:wght@300;400;500;600&display=swap');
.section-four {
    position: absolute;
    width: 100%;
    height: 1003px;
    left: 0px;
    top: 2818px;
    background: linear-gradient(180deg, #333333 0%, #000000 0.01%);
}
.section-four img {
    position: absolute;
    width: 719px;
    height: 423px;
    left: 229px;
    top: 275px;
}
.group-seven {
    position: relative;
    width: 526px;
    height: 734px;
    left: 1082px;
    top: 210px;
    /* top: 3019px; */
}
.contact-title {
    position: absolute;
    top: 0%;
    bottom: 90.05%;
    font-family: 'Kanit', sans-serif;
    font-style: normal;
    font-weight: 500;
    font-size: 60px;
    line-height: 73px;
    text-transform: capitalize;
    color: #FFFFFF;
    height: 73px;
}
.contact-body {
    position: absolute;
    top: 13%;
    bottom: 90.05%;
}
.form-control {
    background-color: black;
    border: none;
    border-bottom: 1px solid white;
    color: white;
    font-family: Arial, sans-serif;
    font-size: 16px;
    padding: 8px 0;
    width: 519.0000000000019px;
    font-family: 'Kanit', sans-serif;
    font-style: normal;
    font-weight: 300;
    font-size: 17px;
    line-height: 22px;
    margin: 18px 0;
}
.form-control::placeholder {
    color: white;
}
.form-calendar {
    position: relative;
}
.form-calendar .icon {
    font-size: 22px;
    position: absolute;
    min-width: 40px;
    right: 0px;
    bottom: 28px;
    cursor: pointer;
}
.contact-detail {
    margin-top: 20px;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 300;
}
.btn {
    position: absolute;
    top: 72.48%;
    bottom: 19.89%;
    background: linear-gradient(180deg, #DEE34B 0%, #D9EF0C 35.94%, #87A30D 100%);
    box-shadow: 0px 4px 10px rgba(0, 0, 0, 0.35);
    border-radius: 50px;
    height: 56px;
    width: 290px;
    left: 0px;
    top: 450px;
    border-radius: 50px;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 500;
    font-size: 20px;
    line-height: 18px;
    text-align: center;
    letter-spacing: 0.1px;
    cursor: pointer;
}
</style>
