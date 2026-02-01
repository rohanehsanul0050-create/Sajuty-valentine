# Sajuty-valentine <!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>For Sajuty ❤️</title>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Segoe UI', sans-serif;
}

body {
  height: 100vh;
  background: linear-gradient(135deg, #ffd1dc, #ff9a9e);
  display: flex;
  justify-content: center;
  align-items: center;
  overflow: hidden;
}

/* Floating hearts */
.heart {
  position: absolute;
  color: rgba(255, 0, 100, 0.4);
  font-size: 20px;
  animation: float 6s infinite ease-in;
}

@keyframes float {
  0% {
    bottom: -10%;
    opacity: 0;
  }
  50% {
    opacity: 1;
  }
  100% {
    bottom: 110%;
    opacity: 0;
  }
}

.card {
  background: rgba(255, 255, 255, 0.9);
  padding: 40px;
  border-radius: 25px;
  text-align: center;
  max-width: 350px;
  box-shadow: 0 20px 40px rgba(255, 0, 100, 0.3);
  animation: pop 1.5s ease;
}

@keyframes pop {
  from {
    transform: scale(0.8);
    opacity: 0;
  }
  to {
    transform: scale(1);
    opacity: 1;
  }
}

h1 {
  color: #e60073;
  margin-bottom: 15px;
}

p {
  color: #555;
  font-size: 16px;
  margin-bottom: 25px;
}

button {
  background: linear-gradient(135deg, #ff5fa2, #ff3366);
  border: none;
  color: white;
  padding: 12px 25px;
  font-size: 18px;
  border-radius: 30px;
  cursor: pointer;
  transition: 0.3s;
}

button:hover {
  transform: scale(1.1);
  box-shadow: 0 10px 20px rgba(255, 0, 100, 0.4);
}

.love {
  display: none;
  margin-top: 20px;
  color: #e60073;
  font-size: 18px;
}
</style>
</head>

<body>

<!-- Hearts -->
<script>
for (let i = 0; i < 25; i++) {
  let heart = document.createElement("div");
  heart.className = "heart";
  heart.innerHTML = "❤️";
  heart.style.left = Math.random() * 100 + "vw";
  heart.style.animationDuration = (Math.random() * 3 + 4) + "s";
  heart.style.fontSize = (Math.random() * 20 + 10) + "px";
  document.body.appendChild(heart);
}
</script>

<div class="card">
  <h1>Sajuty ❤️</h1>
  <p>
    Every heartbeat of mine whispers your name.  
    Every smile of mine belongs to you.  
    <br><br>
    Will you be my Valentine? 🌹
  </p>

  <button onclick="showLove()">Yes 💖</button>

  <div class="love" id="loveText">
    I knew it 🥹❤️  
    You make my world softer, brighter, and more beautiful every day.
  </div>
</div>

<script>
function showLove() {
  document.getElementById("loveText").style.display = "block";
}
</script>

</body>
</html>
