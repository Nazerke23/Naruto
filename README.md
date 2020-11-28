# Naruto
The website created for university project.

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Header</title>
     <!--------FontAwesom-------->
     <link rel="stylesheet" href="./css/all.css">

     <!-------My fonts downloaded from various websites-->
     <link rel="stylesheet" href="./css/fonts.css">
 
     <!------AOS------->
     <link href="https://unpkg.com/aos@2.3.1/dist/aos.css" rel="stylesheet"> 

      <!--====Swiper.js====-->  
    <link rel="stylesheet" href="https://unpkg.com/swiper/swiper-bundle.css">
    <link rel="stylesheet" href="https://unpkg.com/swiper/swiper-bundle.min.css">
 
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Goldman&display=swap');
        @import url('https://fonts.googleapis.com/css2?family=Underdog&display=swap');
        @import url('https://fonts.googleapis.com/css2?family=Josefin+Sans&display=swap');
        @import url('https://fonts.googleapis.com/css2?family=Lexend+Deca&display=swap');
/*=====================GLOBAL=======================*/
*{
    padding: 0;
    margin: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
}

a{
    text-decoration: none;
}

ul{
    list-style-type: none;
}
/*========x============GLOBAL==========x============*/




/*=========X===========HEADER==============X========*/

header{
    width: 100%;
    min-height: 100vh;
    background: url(./4.jpg);
    background-size: cover;
    background-position: center;
}


/*=========================================================================my menu=======*/
.my-menu{
    display: none;
    justify-content: center;
    align-items: center;
    position: absolute;
    z-index: 1;
    width: 100%;
    height: 100%;
    background-color: #071855de;
}

.my-menu:before{
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: 1;
    background-color: #071855de;
    mix-blend-mode: screen;
}

.menu-elements{
    z-index: 1;
    text-align: center;
    font-size: 40px;
}

.menu-elements h2{
    margin: 10px;
    cursor: pointer;
    color: white;
}

.menu-elements h2:hover{
    color: orange;
    transition: 0.6s;
}

/*========================================================================my menu=======*/

/*=====================================TOP=========================*/
.header-top{
    height: 10vh;
}

/*==============hamburger==========================*/
.menu-btn{
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    width: 30px;
    height: 30px;
    cursor: pointer;
    transition: all .5s ease-in-out;
    left: 30px;
    top: 20px;
    z-index: 1;
}

.menu-btn_burger{
    z-index: 1;
    width: 27px;
    height: 4px;
    background: rgb(212, 209, 209);
    border-radius: 50px;
    box-shadow: 0 2px 5px rgba(255, 101, 47, .2);
    transition: all .5s ease-in-out;
}

.menu-btn_burger::before,
.menu-btn_burger::after {
    content: '';
    position: absolute;
    width: 27px;
    height: 4px;
    background: #fff;
    border-radius: 5px;
    box-shadow: 0 2px 5px rgba(255, 101, 47,.2);
    transition: all .5s ease-in-out;
}

.menu-btn_burger::before{
    transform: translateY(-8px);
}

.menu-btn_burger::after{
    transform: translateY(8px);
}

/*====animation======*/
.menu-btn.open .menu-btn_burger{
    transform: translateX(-50px);
    background: transparent;
    box-shadow: none;
}

.menu-btn.open .menu-btn_burger::before{
    transform: rotate(45deg) translate(35px, -35px);
}

.menu-btn.open .menu-btn_burger::after{
    transform: rotate(-45deg) translate(35px, 35px);
}
/*=======x======hamburger===================x==========*/

/*==============Naruto-Saske-Sakura====================*/
.top-words{
    position: relative;
    left: 100px;
    top: -5px;
    width: 50%;
}

.top-words a{
    color: white;
    font-size: 20px;
    font-family: 'Goldman', cursive;
    margin: 0 15px;
}

.top-words a:hover{
    color: orange;
    border-bottom: 2px solid orange;
    transition: .5s;  
}
/*=======x======Naruto-Saske-Sakura=========x==========*/


/*====login logout======*/
.loginout{
    position: absolute;
    top: 25px;
    right: 100px;
    overflow-x: visible;
}

.loginout a{
    font-family: Monotype;
    margin: 5px;
    padding: 6px 20px;
    color:white;
    background-color: #C96B55;
    border: 1px solid white;
    border-radius: 2rem;
    outline: none;
}

.loginout a#login{
    background: transparent;
}

.loginout a#login:hover{
    background-color: #C96B55;
}

/*=xx==login logout===x===*/

/*===========xxxx======================TOP===============xxxxx======*/




/*==================NARUTO UZUMAKI====================*/
.center{
    position: absolute;
    top: 30%;
    width: 40%;
    left: 12%;
    
}

.center h1{
    color: white;
    font-size: 70px;
    margin: 1rem 0;
    font-family: 'Underdog', cursive;
    letter-spacing: 10px;
}
/*========x=========NARUTO UZUMAKI===========x========*/



/*------------------------------------------------------------Navigation right-----*/
.nav-right{
    position: absolute;
    top: 0;
    right: 0;
    width: 5%;
    height: 100vh;
    background-color: #12256993;
    border-left: 0.1px solid grey;
}

.nav-right .logo img{
    width: 100%;
    cursor: pointer;
}

.nav-right .social-icons{
    display: flex;
    flex-direction: column;
    margin-top: 10%;
    margin-bottom: 4rem;
}

.nav-right .social-icons a{
    margin-top: 20%;
    color: white;
    text-align: center;
    font-size: 15px;
}

.nav-right .social-icons a:hover{
    color:orange;
    transition: .5s;
}

.nav-right .right-words{
    color: rgb(255, 255, 255);
}

.nav-right .right-words h3{
    transform: rotate(90deg);
    font-family: Jokerman;
    font-size: 16px;
}

/*--x-------------------------------------------------------------------------------------------------Navigation right--x--*/


/*==================SCROLL DOWN====================*/
.scrolldown{
    position: absolute;
    bottom: 20px;
    left: 50%;
    width: 40px;
    height: 40px;
    transform: translateY(-80px) translateX(-50%) rotate(45deg);
    cursor: pointer;
}

.scrolldown span{
    position: absolute;
    top:0;
    left: 0;
    display: block;
    width: 100%;
    height: 100%;
    border-bottom: 2px solid #fff;
    border-right: 2px solid #fff;
    animation: animate 1.5s linear infinite;
    opacity: 0;
}

.scrolldown span:nth-child(1){
    transform: translate(-10px, -10px);
    animation-delay: -0.4s;
}

.scrolldown span:nth-child(2){
    transform: translate(0, 0);
    animation-delay: -0.2s;
}

.scrolldown span:nth-child(3){
    transform: translate(10px, 10px);
    animation-delay: 0s;
}

@keyframes animate{
    0%{
        top: -5px;
        left: -5px;
        opacity: 0;
    }
    25%{
        top: 0;
        left: 0;
        opacity: 1;
    }
    100%{
        top: 5px;
        left: 5px;
        opacity: 0;
    }
}
/*========x=========SCROLL DOWN===========x========*/

/*=========X===========HEADER==============X========*/



/*=====================SECOND=======================*/

.second-section{
    max-width: 100%;
    padding: 2rem 3rem 0rem;
    min-height: 100vh;
    background-color: #02025ad8;
    color: white;
    font-family: 'Goldman', cursive;
}

.second-section .second-top{
    display: flex;
    justify-content: space-between;
}

.second-section .second-top .reanimate{
    width: 25%;
}

.second-section .second-top .yourdata{
    width: 35%;
}

.second-section .second-card{
    padding: 2rem;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
}

.second-section .second-card .one-card{
    margin: 1rem 1rem;
    width: 45%;
    height: 370px;
    border: 4px dashed white;
}

.second-section .second-card .one-card#startup{
    background: url(./pict/102.jpg);
    background-size: cover;
    background-position: center;
}

.second-section .second-card .one-card#venture{
    background: url(./413842.jpg);
    background-size: cover;
}
/* ===========X=========SECOND==============X======== */



/*=================================================================3=======================*/

.third-section{
    position: relative;
    padding: 2rem 3rem 0rem;
    min-height: 100vh;
    background-color: #02025ad8;
    color: white;
    font-family: 'Goldman', cursive;
}

.third-section .third-content{
    position: absolute;
    top: 140px;
    display: flex;
    justify-content: space-around;
}

.third-section .third-content .sortwareRuns{
   width: 500px;
}

.watch{
    font-size: 16px;
    padding: 10px 20px;
    margin-left: 8rem;
    margin-top: 3rem;
    background: transparent;
    outline: none;
    border-radius: 2rem;
    border: none;
    color: white;
    font-family: 'Goldman', cursive;
    border: 1px solid whitesmoke;
}

.watch:hover{
    outline: none;
    background: orange;
}

.third-section .third-content .third-picture{
    margin-left: 3rem;
    width: 600px;
    height: 400px;
    border: 2px solid white;
    background: url(./pict/fQUVWQT-a7k.jpg);
    background-size: cover;
}


/*===================xxxxxxxx=============================================3===========xxxx=======*/




/*=============MUSIC_SECTION=========================*/

.music-section{
    position: relative;
    top:10%;
    width: 100%;
    height: 90vh;
    display: flex;
    padding: 5vh 0;
    background-color: #02025ad8;
}

.music-section .imgBx{
    position: relative;
    width: 50%;
    height: 100%;
}

.music-section .imgBx:before{
    content: '';
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: linear-gradient(225deg, #460fac, #03a9f4);
    z-index: 1;
    mix-blend-mode: screen;
}

.music-section .imgBx img{
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
}

.music-section .contentBx{
    display: flex;
    width: 50%;
    height: 100%;
    justify-content: center;
    align-items: center;
    position: relative;
}


#main{
    width: 100%;
    position: absolute;
    top:50%;
    left: 50%;
    transform: translate(-50%,-50%);
    z-index: 999;
}

.music-section .contentBx #play{
    position: absolute;
    border: none;
    width: 50px;
    height: 50px;
    background-color:orange;
    border-radius: 50%;
    outline: none;
    cursor: pointer;
    right: 10%; 
    /* transform: translate(-50%,-50%);  */
}

#next,#pre{
    width: 50px;
    height: 50px;
    border: 0;
    background-color:orange;
    border-radius: 50%;
    outline: none;
    cursor: pointer;
    position: absolute;
    /* top:90%;
    left: 60%; */
    /* transform: translate(-10%,-50%); */
} 



#songTitle{
    width:300px;
    text-align: center;
    font-family: monospace;
    font-size: 34px;
    position: absolute;
    top:-20%;
    left: 50%;
    transform: translate(-50%,-50%);
    color: white;
}


#next{
    width: 30px;
    height: 30px;
    left: 80%;
    top:90%;
}
#pre{
    width: 30px;
    height: 30px;
    left: 15%;
    top: 90%;
}

#play img,#next img,#pre img{
    position: absolute;
    top:50%;
    left: 50%;
    transform: translate(-50%,-50%);
    cursor: pointer;
}


@media (max-width:768px){

    .music-section .imgBx{
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
    }

    .music-section .contentBx{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: 100%;
        height: 100%;
        z-index: 1;
        background: transparent;
    }

}

/*========xx=====MUSIC_SECTION=============xx============*/



/*=============CHARACTERS=========================*/

.characters-section {
    background-color: #02025ad8;
    font-family: Helvetica Neue, Helvetica, Arial, sans-serif;
    font-size: 14px;
    color: #fff;
    display: flex;
    justify-content: center;
    align-items: center;
    min-height: 100vh;
 }
 
 .swiper-container {
    width: 100%;
    padding-top: 50px;
    padding-bottom: 50px;
 }
 
 .swiper-slide {
    background-position: center;
    background-size: cover;
    width: 300px;
    height: 300px;
 
 }
 .swiper-slide img
 {
    width: 100%;
    -webkit-box-reflect: below 1px linear-gradient(transparent,transparent, #0005);
 }
 .id
 {
    color: #fff;
    font-size: 20px;
 }

/*=============CHARACTERS=========================*/



/*=================================X============================FOTTER==========X============*/



/* ----------------- Footer --------------------- */

.flex-row{
    display: flex;
    flex-direction: row;    
    flex-wrap: wrap;
}

footer.footer{
    min-height: 60vh;
    background: orange;
    position: relative;
    padding: 0 3rem;
}

footer.footer .container{
    display: grid;
    grid-template-columns: repeat(4, 1fr);
}

footer.footer .container > div{
    flex-grow: 1;
    flex-basis: 0;
    padding: 3rem .9rem;
}

footer.footer .container h2{
    padding-bottom: .7rem;
    color: white;
    font-family: 'Goldman', cursive;
}

footer.footer .container p{
    padding: .6rem 0;
    font-family: 'Lexend Deca', sans-serif;
}

footer.footer .newsletter .form-element{
    background: rgb(185, 103, 9);
    display: inline-block;
}

footer.footer .newsletter .form-element input{
    padding: .5rem .7rem;
    border: none;
    background: transparent;
    color: white;
    font-family: Monotype;
    font-size: 1rem;
    width: 74%;
}

footer.footer .newsletter .form-element span{
    padding-bottom: 1rem;
    background: rgb(101, 108, 207);
    padding: .5rem .7rem;
    cursor: pointer;
}

footer.footer .instagram div > img{
    display: inline-block;
    width: 25%;
    height: 50%;
    margin: .3rem .4rem;
}

footer.footer .follow div i{
    color: white;
    padding: 0 .4rem;
}

footer.footer .follow div i:hover{
    color:rgb(46, 46, 224);
    transition: .5s;
}

footer.footer .rights{
    justify-content: center;
    font-family: 'Josefin Sans', sans-serif;
}

footer.footer .rights h4 a{
    color: white;
}

footer.footer .move-up{
    position: absolute;
    right: 6%;
    top: 50%;
}

footer.footer .move-up span{
    color: rgba(63, 22, 209, 0.719);
}

footer.footer .move-up span:hover{
    color: white;
    cursor: pointer;
}


/*              Viewport less then or equal to 1130px            */

@media only screen and (max-width: 1130px){
   
    footer.footer .container{
        grid-template-columns: repeat(2, 1fr);
    }

    footer.footer .rights{
        padding-bottom: 1rem;
    }

}

/*      x       Viewport less then or equal to 1130px    x 


/*              Viewport less then or equal to 750px            */

@media only screen and (max-width: 750px){
  
    footer.footer .container{
        grid-template-columns: repeat(1, 1fr);
    }

}


/*        x      Viewport less then or equal to 750px       x     */


/*              Viewport less then or equal to 520px            */

@media only screen and (max-width: 520px){
   
    footer.footer .container > div{
        padding:  1rem .9rem !important;
    }

    footer .rights{
        padding: 0 1.4rem;
        text-align: center;
    }


}

/*        x      Viewport less then or equal to 520px       x     */


/* ---------x------- Footer ----------x---------- */


    </style>
</head>
    <body>
            <!--=========================--HEADER----------------------======--->
        <header>
            <!--======--FULL NAV---======--->
            <div class="my-menu">
                <div class="menu-elements">
                    <h2>Music</h2>    
                    <h2>Video</h2>    
                    <h2>Quotes</h2>    
                    <h2>Characters</h2>    
                    <h2>Image Gallery</h2> 
                </div>
             </div>
        <!--=====--x--FULL NAV--x--====-->


        <!--=====-----TOP--------====-->
        <div class="header-top box">
            <div class="menu-btn box"><!--hamburger-->
                <div class="menu-btn_burger"></div>
            </div>
            <div class="top-words box">
                <a href="#">NARUTO</a>
                <a href="#">SASKE</a>
                <a href="#">SAKURA</a>
            </div>
            <div class="loginout box">
                <a href="./login.html" id="login"> Log In</a>
                <a href="./login.html" id="signin"> Sign In</a>
            </div>
        </div>
        <!--=====------TOP--------====-->

        <!--======--CENTER---======--->
        <div class="center box" data-aos="fade-up" data-aos-delay="100">
            <h1>NARUTO</h1>
            <h1>UZUMAKI</h1>
        </div>
        <!--=====--x-CENTER--x--====-->


        <!----NAV RIGHT------>
            <div class="nav-right">
            <div class="logo">
                <img src="./нарназ.png">
            </div>
            <div class="social-icons">
                <a href="#"><i class="fab fa-facebook"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-youtube"></i></a>
            </div>
            <div class="right-words">
                <h3>N</h3>
                <h3>A</h3>
                <h3>Z</h3>
                <h3>E</h3>
                <h3>R</h3>
                <h3>K</h3>
                <h3>E</h3>
                <br>
                <h3>K</h3>
                <h3>U</h3>
                <h3>L</h3>
                <h3>A</h3>
                <h3>N</h3>
            </div>
        </div>
        <!----x--NAV RIGHT--x---->


        <!------------SCROLL DOWN INDICATOR---------->

        <a href="#second-section">
            <div class="scrolldown">
                <span></span>
                <span></span>
                <span></span>
            </div>
        </a>
        

        <!---------x--SCROLL DOWN INDICATOR--x------->

    </header>
    <!--=========================--HEADER----------------------======--->

    
    <section>
        <!---------x--SECOND SECTION--x------->
            <div class="second-section box" id="second-section">
                <div class="second-top box">
                    <div class="reanimate box">
                        <h4>It's serialization began in 1999, when creator</h4>
                        <h1>Kishimoto</h1>
                        <h1>Masashi</h1>
                    </div>
                    <div class="yourdata box">
                        <p>The anime Naruto is about an orphan named Naruto Uzumaki who wanted to become the Hokage,
                            the Strongest Ninja in his village.
                            However that isn't all the series is about.The main theme of the story is TO NEVER GIVE UP, 
                            depicted to us through Naruto and his Nindo.
                        </p>
                    <br>
                    </div>
                </div>
                <hr>
                <div class="second-card">
                    <div class="one-card" id="startup" data-aos="fade-right"  data-aos-delay="500">
                        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Tempore aut eligendi saepe adipisci iste. Quam?</p>
    
                    </div>
                    <div class="one-card" id="venture" data-aos="fade-left" data-aos-delay="500">
                        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Tempore aut eligendi saepe adipisci iste. Quam?</p>
                    </div>
                </div>
            </div>
            <!---------x--SECOND SECTION--x------->
    </section>


    <section>
        <!-- ----------THIRD SECTION---------->
        <div class="third-section">
           <!--=====-----TOP--------====-->
            <div class="header-top" data-aos="fade-down" data-aos-delay="300">
                    <div class="menu-btn"><!--hamburger-->
                        <div class="menu-btn_burger"></div>
                    </div>
                    <div class="top-words">
                        <a href="#">NARUTO</a>
                        <a href="#">SASKE</a>
                        <a href="#">SAKURA</a>
                    </div>
                    <div class="loginout" >
                        <a href="./login.html" id="login"> Log In</a>
                        <a href="./login.html" id="signin"> Sign In</a>
                    </div>
                </div>
        <!--=====------TOP--------====-->
    
            <div class="third-content">
                    <div class="sortwareRuns">
                        <h5>We believe</h5>
                        <h1>What Naruto teaches us?</h1>
                        <h2>-------</h2>
                        <p>It also teaches us about forgiveness,shown when Naruto never holds a grudge against the villagers despite how they treated him and how he forgave even the likes of Orochimaru,despite all they did.
    
                            It tells us that it is Never too late to Go back to the right side.Redemption is always possible,seen when Obito realizes that he had been wrong and helps Team 7.
                            
                            Naruto also teaches us the lesson of peace.</p>
                        <button class="watch">Watch Trailer</button>
                    </div>
                    <div class="third-picture">
                    </div>
            </div>
        </div>
        <!-------x--THIRD SECTION--x--- -->
    </section>

    
<section>
    <!--/*=============MUSIC_SECTION=========================*/-->
    <div class="music-section">
        <div class="imgBx" data-aos="fade-right" data-aos-delay="100">
            <img src="./PPoster1.jpg" alt="">
        </div>
        <div class="contentBx">
            <div id="main">
                <div id="songTitle">====</div>
            </div>
            <button id="play" onclick="playOrPauseSong()"><img src="Pause.png"/></button>
            <button id="pre" onclick="pre()"><img src="Pre.png" height="90%" width="90%"/></button>
            <button id="next" onclick="next()"><img src="Next.png" height="90%" width="90%"/></button>
        </div>
    </div class="music-section">   
    <!--/*=========x===MUSIC_SECTION==============x==========*/-->
</section>


<section>
    <!--/*=============CHARACTERS=========================*/-->
    <div class="characters-section" style = "overflow-x: hidden!important;">
        <div class="swiper-container">
            <div class="swiper-wrapper">
              <div class="swiper-slide"><h4></h4><img src="narut/21.jpg"></div>
              <div class="swiper-slide"><img src="narut/22.jpg"></div>
              <div class="swiper-slide"><img src="narut/23.jpg"></div>
              <div class="swiper-slide"><img src="narut/24.jpg"></div>
              <div class="swiper-slide"><img src="narut/25.jpg"></div>
              <div class="swiper-slide"><img src="./pict/lcaBujtdK90.jpg"></div>
              <div class="swiper-slide"><img src="./pict/NklDEzN6XW0.jpg"></div>
              <div class="swiper-slide"><img src="./pict/AoVjNP-FAVM.jpg"></div>
              <div class="swiper-slide"><img src="./pict/char3.jpg"></div>
              <div class="swiper-slide"><img src="./pict/char2.jpg"></div>
              <div class="swiper-slide"><img src="./pict/char1.jpg"></div>
            </div>
            <!-- Add Pagination -->
            <div class="swiper-pagination"></div>
            <div class="swiper-button-next id"></div>
            <div class="swiper-button-prev id"></div>
          </div>
    </div>
    <!--/*=======x=====CHARACTERS===========x=============*/-->
</section>

  <!-- --------------------------- Footer ---------------------------------------- -->

  <footer class="footer" style="max-width: 100%;">
    <div class="container">
        <div class="about-us" data-aos="fade-right" data-aos-delay="200">
            <h2>About us</h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Accusantium quia atque nemo ad modi officiis
                iure, autem nulla tenetur repellendus.</p>
        </div>
        <div class="newsletter" data-aos="fade-right" data-aos-delay="200">
            <h2>Newsletter</h2>
            <p>Stay update with our latest</p>
            <div class="form-element">
                <input type="text" placeholder="Email"><span><i class="fas fa-chevron-right"></i></span>
            </div>
        </div>
        <div class="instagram" data-aos="fade-left" data-aos-delay="200">
            <h2>Instagram</h2>
            <div class="flex-row">
                <img src="./pict/0GirR-PwzXk.jpg" alt="insta6">
                <img src="./pict/MGoKXEYRjF0.jpg" alt="insta2">
                <img src="./pict/TVArlD9dYsg.jpg" alt="insta3">
            </div>
            <div class="flex-row">
                <img src="./pict/gPlaN7snp6o.jpg" alt="insta4">
                <img src="./pict/LtloLLQSKzo.jpg" alt="insta5">
                <img src="./pict/team 7.jpg" alt="insta1">
            </div>
        </div>
        <div class="follow" data-aos="fade-left" data-aos-delay="200">
            <h2>Follow us</h2>
            <p>Let us be Social</p>
            <div>
                <i class="fab fa-facebook-f"></i>
                <i class="fab fa-twitter"></i>
                <i class="fab fa-instagram"></i>
                <i class="fab fa-youtube"></i>
            </div>
        </div>
    </div>
    <div class="rights flex-row">
        <h4 class="text-gray">
            Copyright ©2020 All rights reserved | made by <a>Nazerke Kulan</a>
        </h4>
    </div>
    <div class="move-up">
        <span><i class="fas fa-arrow-circle-up fa-2x"></i></span>
    </div>
</footer>

<!-- -------------x------------- Footer --------------------x------------------- -->





    
     <!------AOS----->
     <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>

     <!-----JQuery------>
     <script src="./javascript/jquery-3.5.js"></script>

      <!-----Swiper------>
      <script src="https://unpkg.com/swiper/swiper-bundle.js"></script>
      <script src="https://unpkg.com/swiper/swiper-bundle.min.js"></script>

    </body>
    <script>
        //======================THIS IS FOR OUR HAMBURGER MUNU=============
let menuBtn = document.querySelector('.menu-btn');
let menuOpen = false;
let myMenu = document.querySelector('.my-menu');

menuBtn.addEventListener('click', function() {
    if(!menuOpen){
        menuBtn.classList.add('open');
        menuOpen = true;
        myMenu.style.display = "flex";
    }
    else{
        menuBtn.classList.remove('open');
        menuOpen = false;
        myMenu.style.display = "none";
    }
})

//=================================================================

document.querySelector('.logo img').addEventListener('click', function(){
    window.location.reload();
})

//=================================================================


$(document).ready(function () {

   

    // click to scroll top
    $('.move-up span').click(function () {
        $('html, body').animate({
            scrollTop: 0
        }, 1000);
    })

    // AOS Instance
    AOS.init();

});





//=================MUSIC================================================
    
var songs = ["Naruto Uzumaki1.mp3","Naruto Uzumaki2.mp3","Naruto Uzumaki3.mp3", "Naruto Uzumaki4.mp3", "Naruto Uzumaki5.mp3", "Naruto Uzumaki6.mp3"];
    var poster = ["PPoster1.jpg","PPoster2.jpg","PPoster3.jpg", "PPoster4.jpg", "PPoster5.jpg", "PPoster6.jpg"];
    
    var songTitle = document.getElementById("songTitle");
    
    var song = new Audio();
    var currentSong = 0;    // it point to the current song
    
    window.onload = playSong;   // it will call the function playSong when window is load
    
    function playSong(){
        
        song.src = songs[currentSong];  //set the source of 0th song 
        
        songTitle.textContent = songs[currentSong]; // set the title of song
        
        song.play();    // play the song
    }
    
    function playOrPauseSong(){
        
        if(song.paused){
            song.play();
            $("#play img").attr("src","Pause.png");
        }
        else{
            song.pause();
            $("#play img").attr("src","Play.png");
        }
    }
 

    function next(){
        
        currentSong++;
        if(currentSong > 5){
            currentSong = 0;
        }
        playSong();
        $(".imgBx img").attr("src",poster[currentSong]);
    }

    function pre(){
        
        currentSong--;
        if(currentSong < 0){
            currentSong = 5;
        }
        playSong();
        $(".imgBx img").attr("src",poster[currentSong]);

    }


//==========xxx======MUSIC===================xx=============================



//==================SWIPER===============================================
var swiper = new Swiper('.swiper-container', 
{
  effect: 'coverflow',
  grabCursor: true,
  centeredSlides: true,
  slidesPerView: 'auto',
  coverflowEffect: {
    rotate: 20,
    stretch: 0,
    depth: 200,
    modifier: 1,
    slideShadows: true,
  },
  loop:true,
  autoplay: {
     delay: 1500,
     disableOnInteraction: false,
   },
   navigation: {
     nextEl: '.swiper-button-next',
     prevEl: '.swiper-button-prev',
   },
});
//==========xxx======SWIPER===================xx=============================







    </script>
</html>
