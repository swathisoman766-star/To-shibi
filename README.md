# To-shibi
<!DOCTYPE html>
<html>
<head>
<title>For Shibine 💋</title>

<style>
body{
  margin:0;
  height:100vh;
  background:linear-gradient(135deg,#ff9a9e,#fad0c4);
  display:flex;
  justify-content:center;
  align-items:center;
  flex-direction:column;
  font-family:Arial;
  overflow:hidden;
  text-align:center;
}

h1{
  font-size:40px;
  color:white;
  z-index:2;
}

#miss{
  font-size:30px;
  color:white;
  margin-top:20px;
  display:none;
}

.emoji{
  position:absolute;
  top:-50px;
  font-size:30px;
  animation:fall linear infinite;
}

@keyframes fall{
  0%{transform:translateY(-10vh);}
  100%{transform:translateY(110vh);}
}
</style>

</head>

<body>

<h1>shibine ummmahhhh💋😽😌🎀❤️....</h1>
<div id="miss">miss u 🙂❤️</div>

<script>

setTimeout(function(){
document.getElementById("miss").style.display="block";
},3000);

function createEmoji(){
const emoji=document.createElement("div");
emoji.classList.add("emoji");
emoji.innerHTML="😍";

emoji.style.left=Math.random()*100+"vw";
emoji.style.animationDuration=(Math.random()*3+2)+"s";

document.body.appendChild(emoji);

setTimeout(function(){
emoji.remove();
},5000);
}

setInterval(createEmoji,200);

</script>

</body>
</html>
