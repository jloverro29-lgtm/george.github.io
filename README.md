
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Xbox Cloud Gaming Portal</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background-color: #000;
      color: #fff;
    }
    header {
      padding: 20px;
      text-align: center;
      border-bottom: 1px solid #fff;
    }
    h1 {
      margin: 0;
      font-size: 28px;
    }
    .container {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 80vh;
      flex-direction: column;
    }
    button {
      background: white;
      color: black;
      border: none;
      padding: 15px 30px;
      font-size: 16px;
      cursor: pointer;
      transition: 0.3s;
    }
    button:hover {
      background: #ccc;
    }
    iframe {
      width: 90%;
      height: 80vh;
      border: none;
      margin-top: 20px;
      display: none;
    }
  </style>
</head>
<body>

<header>
  <h1>Xbox Game Streaming Portal</h1>
</header>

<div class="container">
  <button onclick="startGaming()">Start Playing</button>
  <iframe id="cloudFrame" src="https://www.xbox.com/play"></iframe>
</div>

<script>
  function startGaming() {
    document.getElementById("cloudFrame").style.display = "block";
  }
</script>

</body>
</html>
