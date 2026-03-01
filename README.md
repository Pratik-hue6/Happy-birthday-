# Happy-birthday-
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Deeya!</title>
<style>
  /* Body setup */
  body {
    margin: 0;
    padding: 0;
    background: pink;
    overflow: hidden;
    font-family: 'Comic Sans MS', cursive, sans-serif;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    height: 100vh;
    text-align: center;
    color: white;
  }

  /* Shimmering rainbow text */
  h1 {
    font-size: 3em;
    font-weight: bold;
    background: linear-gradient(90deg, red, orange, yellow, green, blue, indigo, violet);
    background-size: 400% 400%;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    animation: rainbow 5s linear infinite;
    margin-bottom: 20px;
  }

  @keyframes rainbow {
    0% {background-position: 0% 50%;}
    50% {background-position: 100% 50%;}
    100% {background-position: 0% 50%;}
  }

  /* Paragraph text */
  p {
    font-size: 1.2em;
    line-height: 1.5em;
    max-width: 600px;
    margin: 0 auto;
  }

  /* Floating sparkles */
  .sparkle {
    position: absolute;
    font-size: 2em;
    animation: float 4s linear infinite;
    pointer-events: none;
  }

  @keyframes float {
    0% { transform: translateY(100vh) rotate(0deg); opacity: 1; }
    100% { transform: translateY(-50vh) rotate(360deg); opacity: 0; }
  }

  /* Confetti pieces */
  .confetti {
    position: absolute;
    width: 10px;
    height: 10px;
    background-color: red;
    opacity: 0.8;
    animation: fall 3s linear infinite;
  }

  @keyframes fall {
    0% { transform: translateY(-10vh) rotate(0deg); }
    100% { transform: translateY(110vh) rotate(360deg); }
  }

</style>
</head>
<body>

<h1>🎉 Happy Birthday in advance, Deeya! 🎉</h1>

<p>
I hope your special day is filled with lots of good vibes,<br>
and everything you truly enjoy.<br><br>
Wishing you an amazing year ahead, full of:<br>
- Exciting opportunities<br>
- Memorable moments<br>
- Success in everything you do<br><br>
May God bless you with happiness, health,<br>
and all the good things life has to offer. ✨
</p>

<script>
/* Floating sparkles */
const sparkles = ["✨", "🌟", "💖", "🎈", "🎉"];
for (let i = 0; i < 30; i++) {
  const sparkle = document.createElement("div");
  sparkle.className = "sparkle";
  sparkle.textContent = sparkles[Math.floor(Math.random() * sparkles.length)];
  sparkle.style.left = Math.random() * 100 + "vw";
  sparkle.style.animationDuration = 2 + Math.random() * 3 + "s";
  sparkle.style.fontSize = 16 + Math.random() * 24 + "px";
  document.body.appendChild(sparkle);
}

/* Falling confetti */
const colors = ["#ff4d4d", "#ffb84d", "#ffff4d", "#4dff4d", "#4d4dff", "#b84dff", "#ff4db8"];
for (let i = 0; i < 100; i++) {
  const confetti = document.createElement("div");
  confetti.className = "confetti";
  confetti.style.left = Math.random() * 100 + "vw";
  confetti.style.backgroundColor = colors[Math.floor(Math.random() * colors.length)];
  confetti.style.width = 5 + Math.random() * 10 + "px";
  confetti.style.height = 5 + Math.random() * 10 + "px";
  confetti.style.animationDuration = 3 + Math.random() * 3 + "s";
  document.body.appendChild(confetti);
}
</script>

</body>
</html>
