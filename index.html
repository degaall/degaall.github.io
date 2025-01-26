<!DOCTYPE html>
<html>
<head>
    <title>Mood Checker</title>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <script src="https://telegram.org/js/telegram-web-app.js"></script>
    <style>
        body {
            font-family: Arial, sans-serif;
            padding: 20px;
            background: #f0f2f5;
            margin: 0;
        }
        .container {
            max-width: 600px;
            margin: 0 auto;
        }
        .mood-btn {
            width: 100%;
            padding: 15px;
            margin: 10px 0;
            border: none;
            border-radius: 10px;
            font-size: 18px;
            cursor: pointer;
            transition: transform 0.2s;
        }
        .mood-btn:hover {
            transform: scale(0.98);
        }
        #result {
            padding: 20px;
            background: white;
            border-radius: 10px;
            margin-top: 20px;
            text-align: center;
            display: none;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Как твое настроение? 😊</h1>
        <button class="mood-btn" style="background: #4CAF50;" onclick="setMood('Отличное! 😄', 3)">⭐️⭐️⭐️ Отличное</button>
        <button class="mood-btn" style="background: #FFC107;" onclick="setMood('Нормальное 🙂', 2)">⭐️⭐️ Нормальное</button>
        <button class="mood-btn" style="background: #F44336;" onclick="setMood('Плохое 😞', 1)">⭐️ Плохое</button>
        <div id="result"></div>
    </div>

    <script>
        // Инициализация Telegram WebApp
        const tg = window.Telegram.WebApp;
        tg.expand();
        tg.MainButton.setText("Отправить результат").hide();

        let currentMood = null;

        function setMood(text, score) {
            currentMood = {text, score};
            const result = document.getElementById('result');
            result.style.display = 'block';
            result.innerHTML = `
                <h2>Вы выбрали: ${text}</h2>
                <p>Спасибо за ответ! 🎉</p>
                <small>ID вашего пользователя: ${tg.initDataUnsafe.user?.id || 'не доступен'}</small>
            `;
            tg.MainButton.show();
        }

        // Обработчик основной кнопки
        Telegram.WebApp.onEvent('mainButtonClicked', function(){
            if(currentMood) {
                tg.sendData(JSON.stringify({
                    mood: currentMood.score,
                    user: tg.initDataUnsafe.user
                }));
                tg.close();
            }
        });

        // Отображение кнопки закрытия
        if (tg.platform !== 'unknown') {
            tg.BackButton.show();
            tg.onEvent('backButtonClicked', () => tg.close());
        }
    </script>
</body>
</html>