<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
    <meta name="viewport" content="width =device-width, initial-scale=1" >
    <style>
        *{
    margin: 0;
    padding: 0;
}
#banner{
    background:linear-gradient(rgba(0,0,0,0.5),#2c2d35da),url(image/back.jpg);
    background-size: cover;
    background-position: center;
    height: 100vh;
}
.logo{
    width: 130px;
    position: absolute;
    top: 3%;
    left: 3%;
}
.banner-text{
    text-align: center;
    color: #fff;
    padding-top: 180px;
}
.banner-text h1{
    font-size: 90px;
    font-family: Georgia, 'Times New Roman', Times, serif;
}
.banner-text p{
    font-size: 25px;
    font-style: italic;
}
.banner-btn{
    margin: 70px auto 0;
}
.banner-btn a{
    width: 150px;
    text-decoration: none;
    display: inline-block;
    margin: 0 10px;
    padding: 12px 0;
    color: #fff;
    border: .5px solid#fff;
    position: relative;
    z-index: 1;
    transition: color 0.5s;
}
.banner-btn a span{
    width: 0%;
    height: 100%;
    position: absolute;
    top: 0;
    left: 0;
    background: #fff;
    z-index: -1;
    transition: 0.5s;
}
.banner-btn a:hover span{
    width: 100%;
}
.banner-btn a:hover{
    color: #000;
}
#sidenav{
    width: 250px;
    height: 100vh;
    position: fixed;
    right: -250px;
    top: 0;
    background: #363b4e9f;
    z-index: 2;
    transition: 0.5s;
}
nav ul li{
    list-style: none;
    margin: 50px 20px;
}
nav ul li a{
    text-decoration: none;
    color: #fff;
}
nav a{
    color: aliceblue;
    font-family: Georgia, 'Times New Roman', Times, serif;
    font-size: 20px;
    padding-top:10px;
    padding-bottom: 10px;
    padding-left: 5px;
    padding-right: 5px;
}
#sidenav a:hover{
    background: linear-gradient(45deg,rgb(152, 159, 190) ,rgba(185, 144, 129, 0.781));
    border-radius:5px;
    box-shadow: 0 0 1px black;
}
#menubtn{
    width: 50px;
    height: 50px;
    background: #1a356ea9;
    text-align: center;
    position: fixed;
    right: 30px;
    top: 20px;
    border-radius: 3px;
    z-index: 3;
    cursor: pointer;
}
#menubtn img{
    width: 50px;
    margin-top: .5px;
}
@media screen and (max-width:770px) {
    .banner-text h1{
        font-size:44px;
    }
    .banner-btn a{
        display: block;
        margin: 20px auto;
    }
}
#feature{
    width: 100%;
    padding: 70px 0;
}
.title-text{
    text-align: center;
    padding-bottom: 70px;
}
.title-text p{
    font-size: 20px;
    color:#113331;
    font-weight: bold;
}
.title-text h1{
    font-size: 50px;
}
.feature-box{
    width: 80%;
    margin: auto;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    text-align: center;
}
.features{
    flex-basis: 70%;
}
.features-img{
    flex-basis: 50%;
    margin: auto;
}
.features-img img{
    width: 70%;
}
.features h1{
    text-align: left;
    margin-bottom: 10px;
    font-weight: 100;
    color: aqua;
}
.features-desc{
    display: flex;
    align-items: center;
    margin-bottom: 40px;
}

    </style>
</head>
<body>

    <section id="banner">

        <img src="image/logo.gif" class="logo">

        <div class="banner-text">

            <h1>ONE PIECE</h1>

            <p>Read our latest One Piece Manga here.</p>

            <div class="banner-btn">
                <a href="aboutus.html"><span></span>ABOUT US</a>
                <a href="readmore.html"><span></span>READ MORE</a>
            </div>

        </div>

    </section>

    <div id="sidenav">

        <nav>
            <ul>
                <li><a href="index.html">HOME</a></li>
                <li><a href="features.html">FEATURES</a></li>
                <li><a href="services.html">SERVICES</a></li>
                <li><a href="shop.html">SHOP</a></li>
                <li><a href="news.html">NEWS</a></li>
                <li><a href="settings.html">SETTINGS</a></li>
            </ul>
        </nav>

    </div>

    <div id="menubtn">
        <img src="image/menu.png" id="menu">
    </div>

    <section id="feature">

        <div class="title-text">
            <p>FEAURES</p>
            <h1>Place sadfsdfasdf holder</h1>
        </div>

        <div class="feature-box">

            <div class="features">

                <h1>place holder</h1>

                <div class="features-desc">

                    <div class="feature-icon"></div>

                    <div class="feature-text">
                        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Non aliquid dolore nesciunt.</p>
                    </div>

                </div>

            </div>

            <div class="features-image">
                <img src="image/p1.webp">
            </div>

        </div>

    </section>

    <script>
        
        var menubtn=document.getElementById("menubtn")
        var sidenav=document.getElementById("sidenav")
        var menu=document.getElementById("menu")

        sidenav.style.right="-250px";

        menubtn.onclick=function(){
            if(sidenav.style.right=="-250px"){
               sidenav.style.right="0";
               menu.src="image/close.png";
            }
            else{
                sidenav.style.right="-250px"; 
                menu.src="image/menu.png";
            }
        }
    </script>
    
</body>
</html>
