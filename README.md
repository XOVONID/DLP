<!DOCTYPE html>
<html lang="zh-Hant">
<head>
  <meta charset="UTF-8">
  <title>東龍自動服務系統</title>
  <style>
    body {
      font-family: sans-serif;
      background: #ffffff;
      text-align: center;
      padding: 30px;
    }

    h1 {
      color: #000000;
    }

    input, button {
      padding: 20px;
      font-size: 24px;
      margin: 5px;
      border-radius: 12px;
      border: 3px solid #000000;
    }

    button {
      background-color: #808A86;
      color: #000000;
      cursor: pointer;
    }

    #total {
      margin-top: 30px;
      font-size: 28px;
      color: #333;
    }
  </style>
</head>
<body>
  <h1>自動服務</h1>

  <button onclick="addToTotal(300)">一般照 300 元</button>
  <button onclick="addToTotal(400)">快照 400 元</button>
  <button onclick="addToTotal(100)">加洗一般件 100 元/組</button>
  <button onclick="addToTotal(150)">加洗快件 150 元/組</button>

  <div id="total">總金額：0 元</div>

  <script>
    let total = 0;

    function addToTotal(amount) {
      total += amount;
      document.getElementById("total").innerText = "總金額：" + total + " 元";
    }
  </script>
</body>
</html>


