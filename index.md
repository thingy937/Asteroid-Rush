<html>
  <body>
  <style>
  html, body {
    height: 100%;
    margin: 0;
  }
  body {
    background: #36393f;
    background-image: url(https://raw.githubusercontent.com/thingy937/thingy937.github.io/master/360_F_279795836_SZU2w1gvtn4586ZfLkC2RtQZeL6wOuIh.jpg);
    display: flex;
    align-items: center;
    justify-content: center;
  }
  canvas {
    border: 8px solid black;
  }
  </style>
<body>    
<div class="" style="width:100;height:100;background-color:#03b1fc;background-image:linear-gradient(#03b1fc, #0339fc); border-radius: 10px; box-shadow: 0px 0px 5px 5px black;">
<p>&nbsp;</p>
<p align="center">
<canvas width="600" height="400" id="game"></canvas>
</p>
<script>
var canvas = document.getElementById('game');
var context = canvas.getContext('2d');
var shipY = 225;

// game loop
function loop() {
  requestAnimationFrame(loop);
  shipY = 225;
  
  //draw ship
  var canvas = document.getElementById("game");
  var ship = c.getContext("2d");
  ship.fillRect(30, shipY, 50, 50);

  //draw lines
  var canvas = document.getElementById("game");
  var line = c.getContext("2d");
  line.fillRect(0, 100, 600, 1);
  line.fillRect(0, 200, 600, 1);
  line.fillRect(0, 300, 600, 1);
  
}

// keyboard events
document.addEventListener('keydown', function(e) {

  // up arrow key
  if (e.which === 38) {
    var shipY = shipY - 100;
  }
  // down arrow key
  else if (e.which === 40) {
  	var shipY = shipY + 100;
  }
});

// start the game
requestAnimationFrame(loop);
</script>
<p align="center">
<button title="Go back" style="background-color: transparent; border-radius: 100px; border: 0; cursor: pointer; box-shadow: 0px 0px 5px 5px #03b1fc; width: 50px; height: 50px; padding: 0px 0px;" onclick="history.back()"><img src="https://raw.githubusercontent.com/thingy937/thingy937.github.io/master/kisspng-arrow-computer-icons-encapsulated-postscript-butto-back-icon-5b160a5fdee165.5756415015281711039129(1).png" width="50" height="50"></button>
<button title="Home" style="background-color: transparent; border-radius: 100px; border: 0; cursor: pointer; box-shadow: 0px 0px 5px 5px #03b1fc; width: 50px; height: 50px; padding: 0px 0px;" onclick="location.href='https://thingy937.github.io/'"><img src="https://raw.githubusercontent.com/thingy937/Snake-game-/master/home_circle_icon_137496.png" width="50" height="50"></button>
</p>
<p>&nbsp;</p>
</div>
