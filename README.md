Used for OBS and StreamLabs
<div class="social-overlay">
    <div class="social-item youtube">
        <img src="youtube-icon.png" alt="YouTube">
        <span>"NAME YOUTUBE"</span>#ชื่อช่อง Youtube
    </div>
    <div class="social-item twitch">
        <img src="twitch-icon.png" alt="Twitch">
        <span>"NAME TWITCH"</span>#ชื่อช่อง Twitch
    </div>
    <div class="social-item tiktok">
        <img src="tiktok-icon.png" alt="TikTok">
        <span>"NAME TIKTOK"</span>#ชื่อช่อง TikTok
    </div>
</div>
####CSS####
body {
    background-color: transparent; /* เพื่อให้ Overlay เป็นโปร่งใส */
}

.social-overlay {
    display: flex;
    justify-content: space-around;
    align-items: center;
    width: 100%;
    height: 180px;
    position: absolute;
    bottom: 0;
    animation: slideUp 5s ease-in-out infinite; /* ทำให้ขยับขึ้น-ลง */
}

.social-item {
    display: flex;
    align-items: center;
    padding: 10px;
    background-color: rgba(0, 0, 0, 0.5); /* โปร่งใส */
    border-radius: 10px;
    color: white;
    font-size: 20px;
    font-family: 'Arial', sans-serif;
    animation: pulse 2s infinite; /* ทำให้มีการเคลื่อนไหวเล็กๆ */
}

.social-item img {
    height: 40px;
    margin-right: 10px;
}

/* Animation */
@keyframes slideUp {
    0% { transform: translateY(100px); }
    50% { transform: translateY(0px); }
    100% { transform: translateY(100px); }
}

@keyframes pulse {
    0% { transform: scale(1); }
    50% { transform: scale(1.1); }
    100% { transform: scale(1); }
}
