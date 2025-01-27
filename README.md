# walentynka
<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Walentynka</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            margin-top: 50px;
        }
        .hidden {
            display: none;
        }
        img {
            width: 200px;
            margin-top: 20px;
        }
        button {
            margin: 10px;
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            border: none;
            background-color: #ff6b6b;
            color: white;
            border-radius: 5px;
        }
        button:hover {
            background-color: #ff4c4c;
        }
    </style>
</head>
<body>
    <h1>Zostaniesz moją walentynką?</h1>
    <button onclick="showLove()">Tak</button>
    <button onclick="showNo()">Nie</button>

    <div id="response" class="hidden">
        <img src="https://upload.wikimedia.org/wikipedia/commons/3/35/Teddy_bear_with_red_rose.jpg" alt="Miś z kwiatami">
        <h2>Kocham Cię!</h2>
    </div>

    <div id="rejection" class="hidden">
        <h2>Może zmienisz zdanie?</h2>
    </div>

    <script>
        function showLove() {
            document.getElementById('response').classList.remove('hidden');
            document.getElementById('rejection').classList.add('hidden');
        }

        function showNo() {
            document.getElementById('rejection').classList.remove('hidden');
            document.getElementById('response').classList.add('hidden');
        }
    </script>
</body>
</html>
