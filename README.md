<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Rith ❤️ Rathany</title>

<style>
body{
margin:0;
font-family:sans-serif;
text-align:center;
background:#ffdde1;
overflow:hidden;
}

h1{
margin-top:40px;
color:#ff2e63;
}

.gallery img{
width:80%;
max-width:300px;
border-radius:15px;
margin:10px;
box-shadow:0 10px 20px rgba(0,0,0,0.2);
}

button{
padding:15px 25px;
font-size:18px;
border:none;
border-radius:10px;
background:#ff2e63;
color:white;
margin-top:20px;
}

.heart{
position:fixed;
top:-10px;
color:red;
font-size:20px;
animation:fall 5s linear infinite;
}

@keyframes fall{
0%{transform:translateY(-10px);}
100%{transform:translateY(100vh);}
}
</style>

</head>

<body>

<h1>Rith ❤️ Rathany</h1>
<p>You are the best thing in my life.</p>

<div class="gallery">
<img src="photo1.jpg">
<img src="photo2.jpg">
<img src="photo3.jpg">
</div>

<button onclick="showLove()">Click for Surprise</button>

<audio id="song" autoplay loop>
<source src="song.mp3" type="audio/mpeg">
</audio>

<script>

function showLove(){
alert("I Love You Rathany ❤️");
}

function hearts(){
const heart=document.createElement("div");
heart.classList.add("heart");
heart.innerHTML="❤️";
heart.style.left=Math.random()*100+"vw";
heart.style.animationDuration=(Math.random()*3+2)+"s";
document.body.appendChild(heart);

setTimeout(()=>{heart.remove();},5000);
}

setInterval(hearts,300);

</script>

</body>
</html>
