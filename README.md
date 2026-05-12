{
  "name": "TipTop Unified",
  "short_name": "TipTop",
  "description": "Unified Business Dashboard",
  "start_url": "/TipTop-Unified.html",
  "display": "standalone",
  "background_color": "#18181b",
  "theme_color": "#f43f5e",
  "icons": [
    {
      "src": "icon-192.png",
      "sizes": "192x192",
      "type": "image/png"
    },
    {
      "src": "icon-512.png",
      "sizes": "512x512",
      "type": "image/png"
    }
  ]
}
<link rel="manifest" href="manifest.json">
<meta name="theme-color" content="#f43f5e">
self.addEventListener('install', () => self.skipWaiting());
self.addEventListener('activate', () => self.clients.claim());
<script>
if ('serviceWorker' in navigator) {
  navigator.serviceWorker.register('sw.js');
}
npm init -y
npm install @capacitor/core @capacitor/cli
npx cap init
npx cap add android
npx cap add ios
