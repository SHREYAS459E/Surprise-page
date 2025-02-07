<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Proposing Rose</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background: linear-gradient(135deg, #000000, #434343);
            font-family: 'Arial', sans-serif;
            overflow: hidden;
        }
        .container {
            text-align: center;
            background: rgba(255, 255, 255, 0.1);
            padding: 40px;
            border-radius: 20px;
            backdrop-filter: blur(10px);
            box-shadow: 0 8px 32px rgba(0, 0, 0, 0.2);
            max-width: 600px;
        }
        .rose {
            font-size: 120px;
            animation: float 3s ease-in-out infinite;
            color: #ff007f;
        }
        .message {
            font-size: 32px;
            color: white;
            margin: 20px 0;
            font-weight: bold;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }
        .paragraph {
            font-size: 18px;
            color: white;
            margin: 20px 0;
            line-height: 1.6;
            text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
        }
        .buttons {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 30px;
        }
        .button {
            padding: 15px 40px;
            font-size: 22px;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            font-weight: bold;
            text-transform: uppercase;
        }
        .button.yes {
            background: linear-gradient(135deg, #4CAF50, #45a049);
            color: white;
            box-shadow: 0 4px 15px rgba(76, 175, 80, 0.4);
        }
        .button.yes:hover {
            transform: scale(1.1);
            box-shadow: 0 6px 20px rgba(76, 175, 80, 0.6);
        }
        .button.no {
            background: linear-gradient(135deg, #f44336, #e53935);
            color: white;
            box-shadow: 0 4px 15px rgba(244, 67, 54, 0.4);
            position: relative;
        }
        .button.no:hover {
            transform: translateX(calc(100% + 20px));
            box-shadow: 0 6px 20px rgba(244, 67, 54, 0.6);
        }
        @keyframes float {
            0%, 100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-20px);
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="rose">🌹</div>
        <div class="message">Will you make me the happiest person and be mine forever?</div>
        <div class="paragraph">
            "From the moment our paths crossed, I knew there was something extraordinary about you. Your kindness, intelligence, and unwavering support have brought immense joy and meaning to my life. Every moment spent with you feels like a cherished gift, and I am constantly inspired by your strength and grace. Today, with all my heart, I ask if you would do me the honor of sharing your future with me."
        </div>
        <div class="buttons">
            <button class="button yes" onclick="alert('Yay! You made me the happiest person! ❤️')">Yes</button>
            <button class="button no">No</button>
        </div>
    </div>
</body>
</html>
