---
name: Custom issue template
about: Describe this issue template's purpose here.
title: ''
labels: ''
assignees: ''

---

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document.getElementById("analyzeBtn").addEventListener("click",()=>{
  const input = document.getElementById("roundsInput").value;
  const rounds = input.split(",").map(Number).filter(n=>!isNaN(n));
  if(rounds.length===0){document.getElementById("results").innerText="لا توجد بيانات";}
  else{
    const avg = (rounds.reduce((a,b)=>a+b,0)/rounds.length).toFixed(2);
    const max = Math.max(...rounds);
    const min = Math.min(...rounds);
    document.getElementById("results").innerHTML=`المتوسط: ${avg}<br>أعلى جولة: ${max}<br>أقل جولة: ${min}`;
  }
});const canvas = document.getElementById("simCanvas");
const ctx = canvas.getContext("2d");
let x = 0;
document.getElementById("startSim").addEventListener("click", ()=>{
  x=0;
  animate();
});
function animate(){
  ctx.clearRect(0,0,canvas.width,canvas.height);
  ctx.fillStyle="#00E5FF";
  ctx.fillRect(x,100,50,20); // الطائرة
  x+=2;
  if(x<canvas.width){
    requestAnimationFrame(animate);
  } else {
    ctx.fillStyle="#FF5252";
    ctx.font="20px sans-serif";
    ctx.fillText("انفجار!",150,100);
  }
}body{
  background:#0A0F1F;
  color:white;
  font-family:sans-serif;
  text-align:center;
}
h1{
  color:#00E5FF;
  text-shadow: 0 0 5px #00E5FF;
}
.container{
  max-width:400px;
  margin:50px auto;
  padding:20px;
  background:rgba(0,0,0,0.5);
  border-radius:10px;
}
input, button{
  width:100%;
  margin:10px 0;
  padding:10px;
  border-radius:5px;
  border:none;
}
button{
  background: linear-gradient(90deg,#1E88E5,#00E5FF);
  color:white;
  font-weight:bold;
  cursor:pointer;
}
button:hover{
  opacity:0.8;
}
#errorMsg{
  color:#FF5252;
  font-weight:bold;
}https://username.github.io/airplane_simulator/index.html
