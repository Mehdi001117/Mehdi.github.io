<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>تولدت مبارک موسی! 🎂</title>
    <style>
        body {
            margin: 0;
            background: linear-gradient(45deg, #ff6b6b, #ff8e8e);
            min-height: 100vh;
            font-family: Tahoma;
            text-align: center;
            overflow: hidden;
        }

        h1 {
            color: white;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
            padding: 2rem;
            animation: bounce 2s infinite;
        }

        @keyframes bounce {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-20px); }
        }

        .hearts div {
            position: absolute;
            animation: float 3s linear infinite;
            font-size: 24px;
            color: #ff2768;
        }

        @keyframes float {
            0% { transform: translateY(100vh); }
            100% { transform: translateY(-100vh); }
        }
    </style>
</head>
<body>
    <h1>🎉 تولدت مبارک موسی عزیز! 💖</h1>
    
    <audio autoplay loop>
        <source src="https://cdn.pixabay.com/audio/2023/08/22/audio_5d5b61697e.mp3" type="audio/mpeg">
    </audio>

    <div class="hearts">
        <!-- قلب ها توسط جاوااسکریپت ساخته میشن -->
    </div>

    <script>
        // ساخت قلبهای متحرک
        function createHearts() {
            const container = document.querySelector('.hearts');
            for(let i = 0; i < 20; i++) {
                const heart = document.createElement('div');
                heart.innerHTML = '❤️';
                heart.style.left = Math.random() * 100 + '%';
                heart.style.animationDelay = Math.random() * 2 + 's';
                container.appendChild(heart);
            }
        }

        // فعالسازی صدا با کلیک
        document.addEventListener('click', () => {
            document.querySelector('audio').play();
        });

        window.onload = createHearts;
    </script>
</body>
</html>
