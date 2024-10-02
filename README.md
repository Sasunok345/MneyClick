
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Кликер Монет</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f5f5f5;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            text-align: center;
        }
        #main {
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
            padding: 20px;
            width: 90%;
            max-width: 400px;
        }
        h1 {
            font-size: 24px;
            margin-bottom: 10px;
        }
        #coinCircle {
            width: 100px;
            height: 100px;
            background-color: #FFD700; /* Цвет круга (золотой) */
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            cursor: pointer;
            margin: 20px auto; /* Центрирование круга */
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
            transition: transform 0.2s;
        }
        #coinCircle:hover {
            transform: scale(1.1); /* Увеличение при наведении */
        }
        p {
            font-size: 16px;
            margin-bottom: 20px;
        }
        button {
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            padding: 10px;
            font-size: 16px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
        button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <div id="main">
        <h1>Кликер Монет</h1>
        <div id="coinCircle" onclick="addCoins()">
            <span id="coinCount">0</span> <!-- Количество монет -->
        </div>
        <p>Кликните на круг, чтобы получить монетки!</p>
    </div>

    <script>
        let coins = 0;

        function addCoins() {
            coins++;
            document.getElementById('coinCount').innerText = coins; // Обновление количества монет
        }
    </script>
</body>
</html>
