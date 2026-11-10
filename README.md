index.html.
# jasmeet-birthday

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday Jasmeet!</title>
<style>
* { box-sizing: border-box; }
body {
  margin: 0;
  min-height: 100vh;
  background: linear-gradient(135deg,#090909,#211708,#090909);
  color: white;
  font-family: Georgia, serif;
  text-align: center;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 25px;
}
.card {
  max-width: 550px;
  width: 100%;
  padding: 40px 22px;
  border: 1px solid #c99b35;
  border-radius: 22px;
  box-shadow: 0 0 35px #b8863333;
}
h1 { color: #f2ca70; font-size: 38px; }
p { line-height: 1.8; color: #eee1c5; }
.gift { font-size: 65px; margin: 20px; }
button {
  background: #d6aa51;
  color: #17100a;
  border: none;
  padding: 13px 25px;
  border-radius: 25px;
  font-size: 16px;
  cursor: pointer;
  margin: 10px;
}
button:hover { background: #ffe09a; }
#surprise { display: none; }
.gold { color: #f2ca70; }
</style>
</head>
<body>
<div class="card">
  <div class="gold">✦ A LITTLE SURPRISE ✦</div>
  <div class="gift">🎁</div>
  <h1>Hey Jasmeet!</h1>
  <p>Someone has created a little surprise for you.</p>
  <button onclick="openGift()">Open Your Gift ✨</button>

  <div id="surprise">
    <h1>Happy Birthday! 🎂</h1>
    <p>
      Wishing you a day filled with happiness,
      laughter and beautiful memories.
      May your smile never fade and may
      this year bring you lots of amazing moments.
    </p>
    <h2 class="gold">Stay Happy, Stay Amazing! 💛</h2>
    <p>Here's to another year of wonderful memories!</p>
    <button onclick="showWish()">One More Surprise 💌</button>
    <p id="wish"></p>
  </div>
</div>

<script>
function openGift() {
  document.getElementById("surprise").style.display = "block";
}
function showWish() {
  document.getElementById("wish").innerText =
    "Your final surprise is this: Never stop being your wonderful self! ✨";
}
</script>
</body>
</html>
