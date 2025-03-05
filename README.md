# 8-march
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Переход</title>
    <style>
        body {
            background-color: #1E1E1E;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }
        
        .button {
            background: white;
            color: black;
            padding: 15px 30px;
            border-radius: 8px;
            font-size: 16px;
            font-weight: bold;
            cursor: pointer;
            border: none;
            opacity: 0;
            transform: translateY(10px);
            transition: opacity 0.5s ease-out, transform 0.5s ease-out;
        }

        .button.show {
            opacity: 1;
            transform: translateY(0);
        }

        .button:active {
            transform: translateX(10px);
            opacity: 0;
        }
    </style>
</head>
<body>

    <button class="button" onclick="goToNextPage()">Перейти →</button>

    <script>
        window.onload = function() {
            document.querySelector(".button").classList.add("show");
        };

        function goToNextPage() {
            document.querySelector(".button").style.opacity = "0";
            document.querySelector(".button").style.transform = "translateX(20px)";
            setTimeout(() => {
                window.location.href = "congrats.html"; // Вторая страница
            }, 500);
        }
    </script>

</body>
</html>

<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Поздравление</title>
    <style>
        body {
            background-color: #1E1E1E;
            color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            height: 100vh;
            margin: 0;
            font-family: Arial, sans-serif;
            text-align: center;
        }

        h1 {
            font-size: 32px;
            margin-bottom: 20px;
        }

        p {
            font-size: 20px;
            opacity: 0;
            transform: translateY(10px);
            transition: opacity 1s ease-out, transform 1s ease-out;
        }

        .show {
            opacity: 1;
            transform: translateY(0);
        }
    </style>
</head>
<body>

    <h1>Поздравляем! 🎉</h1>
    <p id="invite">Вы приглашены на наше мероприятие!</p>

    <script>
        window.onload = function() {
            document.getElementById("invite").classList.add("show");
        };
    </script>

</body>
</html>
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Поздравление</title>
    <style>
        body {
            background-color: #1E1E1E;
            color: white;
            display: flex;
            justify-content: center;
            align-items: center;
            flex-direction: column;
            height: 100vh;
            margin: 0;
            font-family: Arial, sans-serif;
            text-align: center;
        }

        h1 {
            font-size: 32px;
            margin-bottom: 20px;
        }

        p {
            font-size: 20px;
            opacity: 0;
            transform: translateY(10px);
            transition: opacity 1s ease-out, transform 1s ease-out;
        }

        .show {
            opacity: 1;
            transform: translateY(0);
        }
    </style>
</head>
<body>

    <h1>Поздравляем! 🎉</h1>
    <p id="invite">Вы приглашены на наше мероприятие!</p>

    <script>
        window.onload = function() {
            document.getElementById("invite").classList.add("show");
        };
    </script>

</body>
</html>

