<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>야시장 메뉴</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background: #fff8f0;
      color: #333;
    }
    header {
      background: #ff6600;
      color: white;
      padding: 1rem;
      text-align: center;
      font-size: 1.5rem;
    }
    .menu {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(160px, 1fr));
      gap: 1rem;
      padding: 1rem;
    }
    .item {
      background: white;
      border-radius: 10px;
      padding: 1rem;
      box-shadow: 0 2px 5px rgba(0,0,0,0.15);
      text-align: center;
      transition: transform 0.2s ease;
    }
    .item:hover {
      transform: scale(1.05);
    }
    .item button {
      margin-top: 0.5rem;
      padding: 0.5rem 1rem;
      background: #ff6600;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      font-size: 1rem;
      width: 100%;
    }
    .item button:hover {
      background: #cc5200;
    }
    footer {
      background: #222;
      color: white;
      text-align: center;
      padding: 1rem;
      margin-top: 1rem;
    }
  </style>
</head>
<body>
  <header>🍢 야시장 메뉴 🍢</header>

  <main class="menu">
    <div class="item">
      <h3>어묵탕</h3>
      <p>₩3,000</p>
      <button onclick="order('어묵탕')">주문하기</button>
    </div>
    <div class="item">
      <h3>닭꼬치</h3>
      <p>₩4,000</p>
      <button onclick="order('닭꼬치')">주문하기</button>
    </div>
    <div class="item">
      <h3>호떡</h3>
      <p>₩2,000</p>
      <button onclick="order('호떡')">주문하기</button>
    </div>
    <div class="item">
      <h3>순대</h3>
      <p>₩3,500</p>
      <button onclick="order('순대')">주문하기</button>
    </div>
  </main>

  <footer>© 2025 야시장. 모든 권리 보유.</footer>

  <script>
    function order(item) {
      alert(item + " 주문이 완료되었습니다!");
    }
  </script>
</body>
</html>
