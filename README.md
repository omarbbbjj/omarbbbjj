<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Football Game with Packs</title>
  <style>
    body { margin: 0; font-family: sans-serif; background: #0b0c10; color: white; text-align: center; }
    #menu, #game, #packs { display: none; padding: 20px; }
    button { padding: 10px 20px; font-size: 16px; margin: 10px; }
    .player-card { background: #1f2833; margin: 10px auto; padding: 10px; width: 200px; border-radius: 8px; }
  </style>
</head>
<body>
  <div id="menu">
    <h1>Football Game</h1>
    <button onclick="startGame()">ابدأ اللعب</button>
    <button onclick="openPackMenu()">فتح بكجات</button>
  </div>  <div id="game">
    <h2>مباراة كرة قدم (عرض فقط)</h2>
    <p>هذه مجرد واجهة مبدأية للمباراة. (3D قيد التطوير)</p>
    <button onclick="goHome()">عودة</button>
  </div>  <div id="packs">
    <h2>فتح بكج</h2>
    <button onclick="openPack()">افتح بكج</button>
    <div id="packResults"></div>
    <button onclick="goHome()">عودة</button>
  </div>  <script>
    const players = ["رونالدو", "ميسي", "محمد صلاح", "نيمار", "هالاند", "بنزيما", "مودريتش"];

    document.getElementById('menu').style.display = 'block';

    function startGame() {
      document.getElementById('menu').style.display = 'none';
      document.getElementById('game').style.display = 'block';
    }

    function openPackMenu() {
      document.getElementById('menu').style.display = 'none';
      document.getElementById('packs').style.display = 'block';
      document.getElementById('packResults').innerHTML = '';
    }

    function goHome() {
      document.getElementById('game').style.display = 'none';
      document.getElementById('packs').style.display = 'none';
      document.getElementById('menu').style.display = 'block';
    }

    function openPack() {
      const result = document.getElementById('packResults');
      result.innerHTML = '';
      for (let i = 0; i < 3; i++) {
        const randomPlayer = players[Math.floor(Math.random() * players.length)];
        const card = document.createElement('div');
        card.className = 'player-card';
        card.textContent = `اللاعب: ${randomPlayer}`;
        result.appendChild(card);
      }
    }
  </script></body>
</html><!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Football Game with Packs</title>
  <style>
    body { margin: 0; font-family: sans-serif; background: #0b0c10; color: white; text-align: center; }
    #menu, #game, #packs { display: none; padding: 20px; }
    button { padding: 10px 20px; font-size: 16px; margin: 10px; }
    .player-card { background: #1f2833; margin: 10px auto; padding: 10px; width: 200px; border-radius: 8px; }
  </style>
</head>
<body>
  <div id="menu">
    <h1>Football Game</h1>
    <button onclick="startGame()">ابدأ اللعب</button>
    <button onclick="openPackMenu()">فتح بكجات</button>
  </div>  <div id="game">
    <h2>مباراة كرة قدم (عرض فقط)</h2>
    <p>هذه مجرد واجهة مبدأية للمباراة. (3D قيد التطوير)</p>
    <button onclick="goHome()">عودة</button>
  </div>  <div id="packs">
    <h2>فتح بكج</h2>
    <button onclick="openPack()">افتح بكج</button>
    <div id="packResults"></div>
    <button onclick="goHome()">عودة</button>
  </div>  <script>
    const players = ["رونالدو", "ميسي", "محمد صلاح", "نيمار", "هالاند", "بنزيما", "مودريتش"];

    document.getElementById('menu').style.display = 'block';

    function startGame() {
      document.getElementById('menu').style.display = 'none';
      document.getElementById('game').style.display = 'block';
    }

    function openPackMenu() {
      document.getElementById('menu').style.display = 'none';
      document.getElementById('packs').style.display = 'block';
      document.getElementById('packResults').innerHTML = '';
    }

    function goHome() {
      document.getElementById('game').style.display = 'none';
      document.getElementById('packs').style.display = 'none';
      document.getElementById('menu').style.display = 'block';
    }

    function openPack() {
      const result = document.getElementById('packResults');
      result.innerHTML = '';
      for (let i = 0; i < 3; i++) {
        const randomPlayer = players[Math.floor(Math.random() * players.length)];
        const card = document.createElement('div');
        card.className = 'player-card';
        card.textContent = `اللاعب: ${randomPlayer}`;
        result.appendChild(card);
      }
    }
  </script></body>
</html>

<!---
omarbbbjj/omarbbbjj is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
