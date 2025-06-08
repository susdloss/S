<!DOCTYPE html>
<html lang="tr">
<head>
  <meta charset="UTF-8">
  <title>Barışalım mı?</title>
  <style>
    body {
      text-align: center;
      font-family: sans-serif;
      margin-top: 100px;
      background-color: #ffe6e6;
    }
    h1 {
      font-size: 2em;
      margin-bottom: 50px;
    }
    button {
      font-size: 20px;
      padding: 15px 30px;
      margin: 20px;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      transition: all 0.3s ease;
    }
    #evet {
      background-color: #8BC34A;
      color: white;
    }
    #hayir {
      background-color: #f44336;
      color: white;
    }
  </style>
</head>
<body>
  <h1>Seni çok özledim... Barışalım mı?</h1>
  <button id="evet">Evet ❤️</button>
  <button id="hayir">Hayır 😢</button>

  <script>
    const evetBtn = document.getElementById("evet");
    const hayirBtn = document.getElementById("hayir");

    let evetSize = 20;
    let hayirSize = 20;

    hayirBtn.addEventListener("click", () => {
      hayirSize = Math.max(5, hayirSize - 2);
      evetSize += 4;
      hayirBtn.style.fontSize = hayirSize + "px";
      evetBtn.style.fontSize = evetSize + "px";
    });

    evetBtn.addEventListener("click", () => {
      alert("Yaa yaşasın! ❤️");
    });
  </script>
</body>
</html>
