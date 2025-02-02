<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Carta para Ti</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f8f8f8;
        }
        .card {
            width: 300px;
            height: 200px;
            background-color: #ffcccc;
            position: relative;
            text-align: center;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
            overflow: hidden;
            cursor: pointer;
        }
        .message {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%) scale(0);
            transition: transform 0.5s ease-in-out;
            font-size: 18px;
            color: #333;
        }
        .card.open .message {
            transform: translate(-50%, -50%) scale(1);
        }
    </style>
</head>
<body>
    <div class="card" onclick="openCard()">
        <div class="message">Perdón flaca, estoy mejorando, y espero que pronto podás verlo ❤️</div>
    </div>
    <script>
        function openCard() {
            document.querySelector('.card').classList.add('open');
        }
    </script>
</body>
</html>
