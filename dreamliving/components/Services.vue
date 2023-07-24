<template>
    <div class="services-container">
        
       <h1 class="title">Our Services</h1>
       <div class="container">
        <div class="gallery">
            <div class="img-box"><h3>Australia</h3></div>
            <div class="img-box"><h3>japan</h3></div>
            <div class="img-box"><h3>UK</h3></div>
            <div class="img-box"><h3>India</h3></div>
        </div>
       </div>
    
    </div>
    </template>
    
    <script>
    export default {
        name: "Services",
    }
    </script>
    
    <style>

    .services-container{
        margin-top: 60px;
    }
    .title{
font-size: 35px;
text-align: center;
    }

    .container{
        width: 100%;
        height: 50vh;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .gallery{
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .img-box{
        width:250px;
        height:250px;
        margin:25px;
        border-radius: 20px;
        background: url(../assets/p1.jpg);
        background-size:cover;
        background-position: center;
        position: relative;
        transition: width 0.5s;

    }
    .img-box:nth-child(2){
        background: url(../assets/p2.jpg);
        background-size:cover;
        background-position: center;
    }
    .img-box:nth-child(3){
        background: url(../assets/p3.jpg);
        background-size:cover;
        background-position: center;
    }
    .img-box:nth-child(4){
        background: url(../assets/p4.jpg);
        background-size:cover;
        background-position: center;
    }

    .img-box h3{
        color: #000;
        position: absolute;
        bottom: 0;
        left: 30px;
        transition: bottom 0.5s;
        
    }
    .img-box:hover{
        width:300px;
        height: 350px;
        cursor: pointer;
    }

    .img-box:hover h3{
        bottom: 25px;
    }

    </style>