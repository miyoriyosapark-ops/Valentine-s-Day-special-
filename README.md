# Valentine-s-Day-special-
A tiny Valentine surprise made with love
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Be My Valentine 💖</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
body {
  margin: 0;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  background: linear-gradient(135deg, #ff758c, #ff7eb3);
  font-family: 'Arial', sans-serif;
}

.card {
  background: white;
  padding: 30px;
  border-radius: 20px;
  text-align: center;
  width: 90%;
  max-width: 350px;
  box-shadow: 0 10px 30px rgba(0,0,0,0.25);
}

h1 {
  color: #ff4d6d;
}

p {
  margin-top: 10px;
  font-size: 18px;
}

.buttons {
  margin-top: 25px;
  position: relative;
}

button {
  padding: 12px 22px;
  border: none;
  border-radius: 30px;
  font-size: 16px;
  cursor: pointer;
}

#yes {
  background: #ff4d6d;
  color: white;
}

#no {
  background: #eee;
  position: absolute;
}
</style>
</head>

<body>

<div class="card">
  <h1>Will you be my Valentine? 💘</h1>
  <p>You have only one correct answer 😌</p>

  <div class="buttons">
    <button id="yes">Yes 😍</button>
    <button id="no">No 🙃</button>
  </div>

  <p id="result"></p>
</div>

<script>
const noBtn = document.getElementById("no");
const yesBtn = document.getElementById("yes");
const result = document.getElementById("result");

noBtn.addEventListener("click", () => {
  const x = Math.random() * 200 - 100;
  const y = Math.random() * 200 - 100;
  noBtn.style.transform = `translate(${x}px, ${y}px)`;
});

yesBtn.addEventListener("click", () => {
  document.body.innerHTML = `
    <div style="
      height:100vh;
      display:flex;
      justify-content:center;
      align-items:center;
      background:linear-gradient(135deg,#ff9a9e,#fad0c4);
      font-family:Arial;
      text-align:center;
      padding:20px;
    ">
      <h1>Yayyyy 💖<br>You’re my Valentine 😍🌹</h1>
    </div>
  `;
});
</script>

</body>
</html>
