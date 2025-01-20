<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>محاكاة هاتف آيفون</title>
  <link rel="stylesheet" href="styles.css">
  <link rel="manifest" href="manifest.json">
</head>
<body>
  <div class="iphone">
    <div class="lock-screen" id="lockScreen">
      <span class="time">10:00</span>
      <span class="swipe-text">مرر لفتح القفل</span>
    </div>
    <div class="screen" id="homeScreen" style="display: none;">
      <div class="status-bar">
        <span>10:00</span>
        <div class="icons">
          <span>📶</span>
          <span>Wi-Fi</span>
          <span>🔋</span>
        </div>
      </div>
      <div class="apps">
        <div class="app" onclick="openApp('📞')">📞</div>
        <div class="app" onclick="openApp('✉️')">✉️</div>
        <div class="app" onclick="openApp('📸')">📸</div>
        <div class="app" onclick="openApp('🌐')">🌐</div>
      </div>
      <div class="home-bar"></div>
    </div>
  </div>
  <script src="script.js"></script>
</body>
</html>