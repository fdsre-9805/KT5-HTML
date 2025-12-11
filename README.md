# KT5-HTML
<!DOCTYPE html>
<html>
<head>
<style>
body {
  margin: 0;
  height: 100vh;
  background: #87CEEB;
  overflow: hidden;
}


body::before {
  content: '';
  position: absolute;
  bottom: 0;
  width: 100%;
  height: 60px;
  background: #333;
}


@keyframes move {
  0% { left: -200px; }
  100% { left: calc(100% - 250px); }
}


#car {
  width: 200px;
  height: 60px;
  position: absolute;
  bottom: 30px;
  left: -200px;
  
 
  background: blue;
  border-radius: 15px 40px 5px 5px;
  
  
  animation: move 4s forwards;
}


#car::before {
  content: '';
  position: absolute;
  top: -25px;
  left: 40px;
  width: 100px;
  height: 30px;
  background: blue;
  border-radius: 15px 15px 0 0;
}


.wheel {
  width: 25px;
  height: 25px;
  background: black;
  border-radius: 50%;
  position: absolute;
  bottom: -12px;
}

#wheel1 { left: 30px; }
#wheel2 { right: 30px; }
</style>
</head>
<body>
<div id="car">
  <div class="wheel" id="wheel1"></div>
  <div class="wheel" id="wheel2"></div>
</div>
</body>
</html>
