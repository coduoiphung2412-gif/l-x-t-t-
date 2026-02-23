# l-x-t-t-
CHÚC MỪNG NĂM MỚI 2026
<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <title>Lì Xì Tết 2026</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1 class="title">Lì Xì Tết 2026 🎉</h1>
    <p class="subtitle">Nhấn vào một bao để nhận lời chúc dành cho học sinh ✨</p>

    <div class="grid">
        <!-- 20 bao lì xì tự động tạo bằng JS -->
    </div>

    <div id="popup" class="popup hidden">
        <div class="popup-box">
            <h2>🎁 Lời Chúc Tết</h2>
            <p id="message"></p>
            <button onclick="closePopup()">Đóng</button>
        </div>
    </div>

    <audio id="sound" src="open.mp3"></audio>

    <script src="script.js"></script>
</body>
</html>
body {
    background: #ffdfba;
    font-family: Arial, sans-serif;
    text-align: center;
    margin: 0;
}

.title {
    margin-top: 20px;
    font-size: 2.5rem;
    color: #d10000;
    font-weight: bold;
}

.subtitle {
    font-size: 1.2rem;
    margin-bottom: 20px;
}

.grid {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    gap: 15px;
    padding: 20px;
    max-width: 800px;
    margin: auto;
}

.lixi {
    width: 100%;
    aspect-ratio: 3/4;
    background: url('lixi.png');
    background-size: cover;
    border-radius: 12px;
    cursor: pointer;
    transition: transform .2s;
}

.lixi:hover {
    transform: scale(1.1);
}

.popup {
    position: fixed;
    top: 0; left: 0;
    width: 100%; height: 100%;
    background: rgba(0,0,0,0.5);
    display: flex;
    justify-content: center;
    align-items: center;
}

.hidden {
    display: none;
}

.popup-box {
    background: white;
    padding: 25px;
    width: 300px;
    border-radius: 10px;
    animation: pop 0.3s ease;
}

@keyframes pop {
    from { transform: scale(0.5); opacity: 0; }
    to { transform: scale(1); opacity: 1; }
}

button {
    padding: 10px 20px;
    background: #d10000;
    color: white;
    border: none;
    border-radius: 6px;
    font-size: 1rem;
    cursor: pointer;
}
