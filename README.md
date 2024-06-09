# LandingPage
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Landing Page</title>
    <link rel="stylesheet" href="style.css">
    <link href="https://cdn.jsdelivr.net/npm/remixicon@4.2.0/fonts/remixicon.css" rel="stylesheet"/>
</head>
<body>
    <div id="main">
        <div class="top">
            <div class="overlay">
                <div class="text">
                    <h1>Images</h1>
                    <div class="image"></div>
                    <div class="rtext">
                        <p>Mesmerizing</p>
                        <p>Astonishing</p>
                    </div>
                    <div class="icons">
                        <i class="ri-twitter-fill"></i>
                        <i class="ri-instagram-fill"></i>
                        <i class="ri-facebook-fill"></i>
                    </div>
                </div>
            </div>

        </div>
        <div class="bottom">
            <div class="b1">
            <h1>Popular</h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quos, tenetur dolore exercitationem nobis aut voluptates cupiditate? Quam enim soluta quod, culpa accusantium iure saepe, minus consequatur obcaecati, assumenda sapiente id.</p>
        </div>
            <div class="b2">
                <div class="up">
                    <h1>Latest</h1>
                    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Fugiat atque, veniam, ipsa, error culpa possimus et saepe tempore fuga voluptate aliquid tempora blanditiis consequuntur neque nesciunt non itaque nostrum quae?</p>
                </div>
                <div class="down">
                    <div class="overlay">
                    <h1>More...</h1>
                </div>
            </div>
            </div>
            <div class="b3">
                <div class="overlay">
                    <p>Privacy Policy</p>
                    <p>Terms and Conditions</p>
                    <p>Contact us</p>
                    <p>About us</p>
                </div>
            </div>
        </div>
    </div>
    
</body>
</html>

//CSS Code
*{
    margin: 0;
    padding: 0;
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    box-sizing: border-box;
}
html,body{
    width: 100%;
    height: 100%;
}
#main{
    width: 100%;
    min-height: 100vh;
}
.top{
    width: 100%;
    min-height: 60vh;
    background-image: url(https://cdn.pixabay.com/photo/2015/04/23/22/00/tree-736885_640.jpg);
    background-size: cover;
    background-position: center;

}
.top .overlay{
    position: relative;
    width: 100%;
    min-height: inherit;
    background-color: rgb(0, 0, 0, 0.295);
}
.text{
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: absolute;
    width: 100%;
    padding: 0 10vh;
    color: white;
    bottom: 5%;
}
.text h1{
    font-weight: 600;
    font-size: 4vw;
}
.text .image{
    background-image: url(https://cdn.pixabay.com/photo/2014/02/27/16/10/flowers-276014_640.jpg);
    background-size: cover;
    background-position: center;
    height: 300px;
    width: 220px;
}
#rtext{
    display: flex;
    width: 25%;
    align-items: center;
    justify-content: space-between;
}
.rtext p{
    font-size: 12px;
}
.bottom{
    display: flex;
    width: 100%;
    min-height: 40vh;
}
.b1{
    width: 30%;
    min-height: inherit;
    background-image: url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRAOk_Z2l6Qsdg6BO3fhHSJZs1O3Wv4QQknng&s);
    background-size: cover;
    background-position: center;
}
.b1 h1{
    text-align: center;
    padding: 30px;
}
.b1 p{
    color: white;
    text-align: center;
    padding: 15px;
}
.b2{
    width: 30%;
    min-height: inherit;
    display: flex;
    flex-direction: column;
}
.b2 .up{
    width: 100%;
    min-height: 20vh;
    background-image: url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcShfrLRLJDTroCqhzzPtqh-4kjWA5L1JmBKbg&s);
    background-size: cover;
    background-position: center;
}
.b2 .up h1{
    text-align: center;
    padding: 30px;
}
.b2 .up p{
    color: white;
    text-align: center;
    padding: 15px;
}
.b2 .down{
    width: 100%;
    min-height: 20vh;
    background-image: url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSrjaytODCF4_Mttx6jHKSQvh0IWyhPLswb6g&s);
    background-size: cover;
    background-position: center;

}
.b2 .down .overlay{
    position: relative;
    width: 100%;
    min-height: 20vh;
    background-color: rgb(255,255,255,0.344);
}
.b3{
    width: 40%;
    min-height: inherit;
    background-image: url(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSrYp-1syx7WG1seZMLwzwRGnXUC0Ts7kd6gQ&s);
    background-size: cover;
    background-position: center
}
.b3 .overplay{
    justify-content: right;
    position: relative;
    margin-left: 50%;
    width: 50%;
    height: 100%;
    padding: 4vw 3vh;

}
.b3 .overlay p{
    padding: 1.2vh;
}
@media(max-width:700px){
    .rtext{
        flex-direction: column;
    }
    .b3 .overlay{
        width: 100%;
        margin-left: initial;
    }
}
@media(max-width:500px){
    .text{
        flex-direction: column;
        align-items: flex-start;
    }
    .text h1{
        font-size: 5vh;
    }
    .text .image{
        height: 200px;
        width: 140px;
        margin-top: 20px;
    }
    .rtext{
        flex-direction: column;
        align-items: flex-start;
    }
    .rtext p{
        margin-top: 10px;
    }
    .icon{
        margin-top: 10px;
    }
    .bottom{
        flex-direction: column;
        align-items: flex-start;
    }
    .b1{
        width: 100%;
        min-height: 30vh;
    }
    .b2{
        width: 100%;
    }
    .b2 up{
        min-height: 40vh;
    }
    .b3{
        width: 100%;
        min-height: 30vh;
        background-position: left;
    }
}
