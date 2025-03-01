<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday Norah</title>
    
    <!-- استيراد الخطوط الجديدة -->
    <link href="https://fonts.googleapis.com/css2?family=Parisienne&family=Cookie&display=swap" rel="stylesheet">

    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: black;
            color: white;
            font-family: 'Arial', sans-serif;
            flex-direction: column;
            text-align: center;
            overflow: hidden;
            position: relative;
        }

        /* خلفية النجوم */
        .stars {
            position: absolute;
            width: 100%;
            height: 100%;
            background: url('https://www.transparenttextures.com/patterns/stardust.png') repeat;
            opacity: 0.7;
            animation: moveStars 100s linear infinite;
            z-index: 1;
        }

        @keyframes moveStars {
            from { background-position: 0 0; }
            to { background-position: 1000px 1000px; }
        }

        .heart-container {
            position: relative;
            display: flex;
            flex-direction: column;
            align-items: center;
            z-index: 2;
        }

        .heart {
            width: 200px;
            height: 200px;
            position: relative;
            animation: heartbeat 1.5s infinite ease-in-out;
        }

        @keyframes heartbeat {
            0% { transform: scale(1); }
            50% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }

        .heart svg {
            width: 100%;
            height: 100%;
            fill: red;
            filter: drop-shadow(0 0 20px rgba(255, 0, 0, 0.8));
        }

        .letter {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            font-size: 70px;
            font-weight: bold;
            color: white;
            font-family: 'Cookie', cursive; /* خط جديد لحرف N */
            text-shadow: 0 0 15px rgba(255, 255, 255, 0.9), 0 0 20px rgba(255, 0, 0, 0.8);
        }

        .message {
            font-size: 36px;
            color: red;
            margin-top: 80px;
            font-weight: bold;
            text-shadow: 0 0 10px rgba(255, 0, 0, 0.8);
            font-family: 'Parisienne', cursive; /* تم تغيير الخط */
        }

        .birthday-message {
            font-size: 30px;
            color: white;
            margin-top: 10px;
            font-family: 'Cookie', cursive;
            text-shadow: 0 0 10px rgba(255, 255, 255, 0.8), 0 0 20px rgba(255, 255, 255, 0.5);
        }

        .heart-container:hover .message,
        .heart-container:hover .birthday-message {
            opacity: 1;
        }
    </style>
</head>
<body>

    <div class="stars"></div> <!-- النجوم المتحركة -->

    <div class="heart-container">
        <div class="heart">
            <svg viewBox="0 0 32 29.6">
                <path d="M23.6,0c-2.5,0-4.9,1-6.6,2.8C15.3,1,12.9,0,10.4,0C4.7,0,0,4.7,0,10.4c0,4,2.6,7.4,6.1,10.6
                c3.2,2.9,7.3,5.6,9.3,6.6c2-1,6.1-3.6,9.3-6.6c3.6-3.2,6.1-6.6,6.1-10.6C32,4.7,27.3,0,23.6,0z"/>
            </svg>
            <div class="letter">N</div>
        </div>
        <div class="message">To my life Norah</div>
        <div class="birthday-message">Happy Birthday</div>
    </div>

</body>
</html>
