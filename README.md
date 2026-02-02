# sajuty--valentine <!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>For Sajuty 💖</title>

<style>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family:'Segoe UI', cursive;
}

body{
  height:100vh;
  background:linear-gradient(135deg,#ffd6e8,#ff9acb);
  display:flex;
  justify-content:center;
  align-items:center;
  overflow:hidden;
}

/* floating hearts */
.heart{
  position:absolute;
  font-size:20px;
  animation:float 6s infinite ease-in;
  opacity:0.8;
}

@keyframes float{
  0%{bottom:-10%;opacity:0;}
  50%{opacity:1;}
  100%{bottom:110%;opacity:0;}
}

.card{
  background:rgba(255,255,255,0.95);
  padding:40px;
  border-radius:30px;
  text-align:center;
  width:360px;
  box-shadow:0 25px 50px rgba(255,0,120,0.4);
  animation:pop 1.3s ease;
}

@keyframes pop{
  from{transform:scale(0.7);opacity:0;}
  to{transform:scale(1);opacity:1;}
}

h1{
  color:#ff2f92;
  margin-bottom:15px;
}

p{
  color:#555;
  font-size:16px;
  margin-bottom:25px;
}

.buttons{
  display:flex;
  justify-content:center;
  gap:20px;
}

button{
  padding:12px 25px;
  font-size:17px;
  border-radius:30px;
  border:none;
  cursor:pointer;
  transition:0.3s;
}

#yes{
  background:linear-gradient(135deg,#ff5fa2,#ff2f92);
  color:white;
}

#yes:hover{
  transform:scale(1.1);
}

#no{
  background:#ffc1dd;
  color:#ff2f92;
  position:relative;
}

.love{
  display:none;
  margin-top:20px;
  font-size:18px;
  color:#ff2f92;
}
</style>
</head>

<body>

<!-- 🎵 Ed Sheeran - Perfect (autoplay) -->
<iframe width="0" height="0"
src="https://www.youtube.com/embed/2Vv-BfVoq4g?autoplay=1&loop=1&playlist=2Vv-BfVoq4g"
frameborder="0"
allow="autoplay">
</iframe>

<script>
/* hearts animation */
for(let i=0;i<30;i++){
  let h=document.createElement("div");
  h.className="heart";
  h.innerHTML="💖";
  h.style.left=Math.random()*100+"vw";
  h.style.animationDuration=(Math.random()*3+4)+"s";
  h.style.fontSize=(Math.random()*18+12)+"px";
  document.body.appendChild(h);
}
</script>

<div class="card">
  <h1>Sajuty 💕</h1>

  <p>
    I found a love… for me 💖  
    Tumi jokhon haso, amar shob dukkho theme jay 🌸  
    Tumi amar shob theke shundor golpo…  
    <br><br>
    Sajuty, will you be my Valentine? 🌹
  </p>

  <div class="buttons">
    <button id="yes" onclick="yesLove()">Yes 💖</button>
    <button id="no" onmouseover="moveNo()">No 🙈</button>
  </div>

  <div class="love" id="loveText">
    I knew it 🥹❤️  
    Tumi amar shob theke boro blessing,  
    amar aaj, amar agami 💐
  </div>
</div>

<script>
function yesLove(){
  document.getElementById("loveText").style.display="block";
}

function moveNo(){
  const no=document.getElementById("no");
  no.style.position="absolute";
  no.style.left=Math.random()*70+"%";
  no.style.top=Math.random()*70+"%";
