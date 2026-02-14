```
valentine.html

```
  
<!DOCTYPE html>  
<html lang="en">  
<head>  
<meta charset="UTF-8">  
<title>Be My Valentine</title>  
  
<style>  
body{  
  margin:0;  
  height:100vh;  
  display:flex;  
  flex-direction:column;  
  justify-content:center;  
  align-items:center;  
  background:#ffe6ee;  
  font-family:Arial;  
}  
  
h1{color:#d6336c}  
  
button{  
  padding:12px 25px;  
  font-size:18px;  
  border:none;  
  border-radius:10px;  
  cursor:pointer;  
}  
  
#yes{  
  background:#ff4d6d;  
  color:white;  
}  
  
#no{  
  position:absolute;  
  background:#555;  
  color:white;  
}  
  
#popup{  
  display:none;  
  position:fixed;  
  inset:0;  
  background:rgba(0,0,0,.6);  
  justify-content:center;  
  align-items:center;  
}  
  
#box{  
  background:white;  
  padding:30px;  
  border-radius:15px;  
  text-align:center;  
  font-size:22px;  
}  
</style>  
</head>  
  
<body>  
  
<h1>Can you be my Valentine? 💖</h1>  
  
<div>  
<button id="yes">Yes</button>  
<button id="no">No</button>  
</div>  
  
<div id="popup">  
  <div id="box">  
    🌹🌹🌹🌹🌹<br>  
    I knew you'd say YES 😍<br>  
    Happy Valentine habibti 💕<br>  
    🌹🌹🌹🌹🌹  
  </div>  
</div>  
  
<script>  
const noBtn = document.getElementById("no");  
const yesBtn = document.getElementById("yes");  
const popup = document.getElementById("popup");  
  
noBtn.addEventListener("mouseover", ()=>{  
  noBtn.style.left = Math.random()*80 + "%";  
  noBtn.style.top  = Math.random()*80 + "%";  
});  
  
yesBtn.addEventListener("click", ()=>{  
  popup.style.display="flex";  
});  
</script>  
  
</body>  
</html>  
