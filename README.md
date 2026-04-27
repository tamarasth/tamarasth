<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Tamara's Coding Corner</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;700&display=swap" rel="stylesheet">

<style>
body {
  margin: 0;
  overflow: hidden;
  font-family: 'Poppins', sans-serif;
  background: linear-gradient(135deg, #1a002f, #3a0ca3, #7209b7);
  color: white;
  text-align: center;
}


.content {
  position: relative;
  z-index: 2;
  padding: 60px 20px;
  max-width: 800px;
  margin: auto;
}


h1 {
  font-size: 3em;
  margin-bottom: 10px;
}

h2 {
  margin-top: 40px;
  color: #c77dff;
}


p {
  font-size: 1.2em;
}

ul {
  list-style: none;
  padding: 0;
}

li {
  margin: 8px 0;
}


.badges img {
  margin: 5px;
}


.ball {
  position: absolute;
  width: 10px;
  height: 10px;
  border-radius: 50%;
  animation: fall linear infinite;
}

@keyframes fall {
  0% {
    transform: translateY(-100px);
    opacity: 1;
  }
  100% {
    transform: translateY(100vh);
    opacity: 0;
  }
}
</style>
</head>

<body>

<div class="content">

  <h1>💜⚡ Welcome to My Coding Corner</h1>
  <p>👋 Hi, I'm Tamara</p>
  <p><strong>Web Developer • Digital Storyteller</strong></p>

 
  <div class="badges">
    <img src="https://img.shields.io/badge/Code-HTML-orange">
    <img src="https://img.shields.io/badge/Style-CSS-purple">
    <img src="https://img.shields.io/badge/Logic-JavaScript-yellow">
  </div>

 
  <h2>💻 About Me</h2>
  <ul>
    <li>🎓 Web Development major</li>
    <li>🌐 Learning: HTML • CSS • JavaScript • PHP • MySQL and more</li>
    <li>🧪 Building small apps and breaking them 5 minutes later</li>
    <li>✨ Obsessed with anything glowing and mystical</li>
    <li>✍️ Horror & fantasy writer (coding by day, summoning demons by night)</li>
    <li>😆 Professional drama-watcher and code-chaos survivor</li>
  </ul>


  <h2>⚡ Current Goals</h2>
  <ul>
    <li>Build a personal portfolio website</li>
    <li>Create dynamic full-stack projects</li>
    <li>Learn cleaner Git workflows</li>
    <li>Get better at debugging without tears 💀</li>
  </ul>




  <h2>🌙 Fun Facts</h2>
  <ul>
    <li>I love drawing (digital and hand-drawn), and designing</li>
    <li>I watch way too many dramas</li>
  </ul>

</div>

<script>
function createBall() {
  const ball = document.createElement("div");
  ball.classList.add("ball");

  ball.style.left = Math.random() * window.innerWidth + "px";
  ball.style.backgroundColor =
    "hsl(" + Math.random() * 360 + ", 100%, 70%)";

  ball.style.animationDuration = (Math.random() * 3 + 2) + "s";

  document.body.appendChild(ball);

  setTimeout(() => {
    ball.remove();
  }, 5000);
}

setInterval(createBall, 200);
</script>

</body>
</html>
