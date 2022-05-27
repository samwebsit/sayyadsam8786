<!DOCTYPE html>
<html>
<head>
<title></title>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css"/>
<style type="text/css">
@import url('https://fonts.googleapis.com/css?family=Luckiest+Guy');
body
{
    margin: 0;
    padding: 0;
    width: 100%;
    height: 100vh;
    font-family: sans-serif;
    
}
.sam
{
    width: 100%;
    height: 100%;
    overflow: hidden;
    position: relative;
    background-image: url("https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTa66TdrxBiSa25xLnhvaN1aXih0uP_R6jYiA&usqp=CAU");
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    text-align:100%;
    justify-content: center;
    animation: change 30s infinite ease-in-out;
}
@keyframes change
{
    0%
    {

    }
    20%
    {
        background-image: url("https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTtVeqwrZTxGqiGwPKFh9iuN6THafJU4ANayQ&usqp=CAU");
    }
    40%
    {
        background-image: url("https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcShhuU4eXpqS_-S5pG-sQj9a19Z1XUqpFZtxg&usqp=CAU");
    }
    60%
    {
        background-image: url("https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTqnUVzU3Ef1FqGgrjV3BVn0iTzCbTYes9afw&usqp=CAU");
    }
    80%
    {
        background-image: url("https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSlEDInT1edAvC2EFG4po-INObDp0wp23axkg&usqp=CAU");
    }
    100%
    {
    
        background-image: url("https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSjEboGkuYR7C5xTk6lNmz427AuNmTnH3XzYQ&usqp=CAU");
    }
}
.sami
{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
}

.wrapper
{
  position:fixed;
  top: 0;
  left: 0;
  height: 100%;
  width: 100%;
  /background: linear-gradient(-135deg, #c850c0, #4158d0);/
  background: linear-gradient(375deg, #1cc7d0, #2ede98); 
 /* clip-path: circle(25px at calc(0% + 45px) 45px); */
  clip-path: circle(25px at calc(100% - 45px) 45px);
  transition: all 0.3s ease-in-out;
}
#active:checked ~ .wrapper
{
  clip-path: circle(100%);
}
.menu-btn{
  position: absolute;
  z-index: 2;
 right: 20px;
 /* left: 20px; */
  top: 30px;
  height: 100px;
  width: 100px;
  text-align: center;
  line-height: 100px;
  border-radius: 100%;
  font-size: 60px;
  color: #fff;
  cursor: pointer;
  background: linear-gradient(-135deg, #c850c0, #4158d0);
  /*background: linear-gradient(375deg, #1cc7d0, #2ede98); */
  transition: all 0.3s ease-in-out;
}
#active:checked ~ .menu-btn{
  background: #fff;
  color: #4158d0;
}
#active:checked ~ .menu-btn i:before{
  content: "\f00d";
}
.wrapper ul{
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  list-style: none;
  text-align:center;
}
.wrapper ul li{
  margin: 50px 0;
}
.wrapper ul li a{
  color: none;
  text-decoration: none;
  font-size: 5em;
  font-weight: 1000;
  padding:30px 0;
  color: #fff;
  position: relative;
  line-height: 100px;
  transition: all 0.3s ease;
}
.wrapper ul li a:after{
  position:fixed;
  content: "";
  background: #fff;
  width: 120%;
  height: 120px;
  left: 0;
  border-radius: 1900px;
  transform: scaleY(0);
  z-index: -1;
  transition: transform 0.3s ease;
}
.wrapper ul li a:hover:after{
  transform: scaleY(1);
}
.wrapper ul li a:hover{
  color: #4158d0;
}
input[type="checkbox"]
{
  display: none;
}
.sami.content{
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  z-index: -1;
  text-align: center;
  width: 100%;
  color: #202020;
}
.sami.content .title{
  font-size: 40px;
  font-weight: 700;
}
.content p{
  font-size: 35px;
  font-weight: 600;
}
@import url('https://fonts.googleapis.com/css?family=Poppins:400,500,600,700&display=swap');
{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Poppins', sans-serif;
}
.h{font-size:4.5em;padding-top:0; margin-top:0px;}


.h1 {

  background-image: url("https://i.pinimg.com/originals/7f/0e/79/7f0e79f225bb91eff5a78ea238898fb3.gif");
  background-size: cover;
  background-clip: text;
  -webkit-background-clip: text;
  color: transparent;
 font-family: 'Luckiest Guy',cursive;
 
 font-size:9.5em;}
 
 
 
.h2{color:#4c0140;text-align:left;font-family:cursive;font-weight:69;font-size:4.5em;}
.h22{font-size:1.5em;font-family:cursive; text-align:center;color:#4c0140;}
</style>
</head>
<body>
<div class="sam">
<input type="checkbox" id="active">    
    <label for="active" class="menu-btn">
       <i class="fas fa-bars">
       </i>
    </label>
<div class="wrapper">
    <div class="sami">
   <ul>
      <li><a href="#"> PROJECT</a></li>
      <li><a href="#"> ABOUT</a></li>
      <li><a href="#"> GUIDANCE</a></li>
      <li><a href="#"> FEEDBACK</a></li>
   </ul>
</div>
</div>
<div class="content">
    <div class="title">
        <br><br><br><br><br><br><br><br><br><br><br><br><br><br>
         <h2 class="h2">Hello..!,I'M SAMIYA </h2>
         <center> <h1 class="h1"> <strike>WEL</strike>COME <br>TO <br>MY <br>WEBSITE</h1>
         <h1 class="h">&#128578;&#128578;&#128578;</center></h1>
         <center><img src="https://miro.medium.com/max/1400/1*vJjJ3Mdok6Rvxx85IIRqBQ.gif" height="350" width="600"></center>
            <br><br><br><br><br><br>
        <hr width="790"size="6">
            <br><br><br><br>
        <center><h2 class="h22">Created By SAMIYA SIKANDER SAYYAD</h2></center>
    </div>  
</div>
</div>
</body>
</html>
