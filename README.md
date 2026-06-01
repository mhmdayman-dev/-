<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>❤️ Our Story ❤️</title>

<style>
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:Arial,sans-serif;
}

body{
background:linear-gradient(135deg,#ff4d6d,#ff758f,#ff8fab);
min-height:100vh;
overflow-x:hidden;
text-align:center;
color:white;
padding:20px;
}

.container{
max-width:900px;
margin:auto;
}

h1{
font-size:3rem;
margin-top:20px;
margin-bottom:15px;
}

.message{
font-size:1.3rem;
line-height:2;
margin-bottom:20px;
}

.counter{
background:rgba(255,255,255,0.15);
padding:20px;
border-radius:20px;
margin:20px auto;
max-width:500px;
backdrop-filter:blur(10px);
font-size:1.4rem;
}

.gallery{
display:flex;
flex-wrap:wrap;
justify-content:center;
gap:15px;
margin-top:25px;
}

.gallery img{
width:280px;
height:350px;
object-fit:cover;
border-radius:20px;
box-shadow:0 0 15px rgba(0,0,0,.2);
}

button{
margin-top:25px;
padding:15px 35px;
border:none;
border-radius:30px;
font-size:18px;
cursor:pointer;
background:white;
color:#ff4d6d;
font-weight:bold;
}

button:hover{
transform:scale(1.05);
}

.heart{
position:fixed;
bottom:-20px;
font-size:25px;
animation:float 8s linear infinite;
opacity:.7;
}

@keyframes float{
0%{
transform:translateY(0);
opacity:0;
}
20%{
opacity:1;
}
100%{
transform:translateY(-110vh);
opacity:0;
}
}
</style>
</head>

<body>

<div class="container">

<h1>❤️ Our Story ❤️</h1>

<div class="message">
أول مرة قولتلك فيها بحبك كانت يوم
<strong>18 / 2 / 2025</strong>
❤️
<br><br>
ومن اليوم ده وكل لحظة بقت أجمل بوجودك.
</div>

<div class="counter">
مر على أول "بحبك" :
<br><br>
<span id="days">0</span> يوم ❤️
</div>

<button onclick="showMessage()">
اضغط هنا ❤️
</button>

<div class="gallery">
<img src="https://images.unsplash.com/photo-1516589178581-6cd7833ae3b2?w=800">
<img src="https://images.unsplash.com/photo-1518199266791-5375a83190b7?w=800">
<img src="https://images.unsplash.com/photo-1524504388940-b1c1722653e1?w=800">
</div>

</div>

<script>
const startDate = new Date("2025-02-18");

function updateCounter(){
const now = new Date();
const diff = now - startDate;
const days = Math.floor(diff / (1000*60*60*24));
document.getElementById("days").innerText = days;
}

updateCounter();

function showMessage(){
alert("❤️ بحبك وهفضل أحبك ❤️");
}

function createHeart(){
const heart = document.createElement("div");
heart.classList.add("heart");
heart.innerHTML="❤️";
heart.style.left=Math.random()*100+"vw";
heart.style.fontSize=(20+Math.random()*30)+"px";
heart.style.animationDuration=(5+Math.random()*5)+"s";
document.body.appendChild(heart);

setTimeout(()=>{
heart.remove();
},10000);
}

setInterval(createHeart,500);
</script>

</body>
</html># -
