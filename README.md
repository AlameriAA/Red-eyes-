// استدعاء العناصر
const lockScreen = document.getElementById("lockScreen");
const homeScreen = document.getElementById("homeScreen");

// فتح الشاشة عند النقر
lockScreen.addEventListener("click", () => {
  lockScreen.style.display = "none";
  homeScreen.style.display = "block";
});

// فتح التطبيق
function openApp(appName) {
  alert(`فتح التطبيق: ${appName}`);
}

// تسجيل الـ Service Worker
if ('serviceWorker' in navigator) {
  navigator.serviceWorker.register('/service-worker.js').then(() => {
    console.log('Service Worker Registered');
  });
}