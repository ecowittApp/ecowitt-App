<link rel="canonical" href="https://ecowittapp.dl7ag.de/">

<style>
:root { color-scheme: dark; }

body {
  background:#0d1117;
  color:#e6edf3;
  font-family:-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,Inter,Helvetica,Arial,sans-serif;
  margin:0;
}

a { color:#58a6ff; text-decoration:none; }
a:hover { text-decoration:underline; }

.wrap {
  max-width:920px;
  margin:0 auto;
  padding:32px 16px 64px;
}

.header {
  text-align:center;
  margin-bottom:20px;
}

.app-icon {
  width:96px;
  height:96px;
  border-radius:22px;
  box-shadow:0 12px 30px rgba(0,0,0,.45);
  margin-bottom:14px;
}

.hero {
  background:rgba(255,255,255,0.03);
  border:1px solid #30363d;
  border-radius:18px;
  padding:28px 22px 26px;
  margin-bottom:18px;
  text-align:center;
}

.hero h1 {
  margin:0 0 6px;
  font-size:2.1rem;
  color:#f0f6fc;
}

.badge {
  display:inline-block;
  margin-left:8px;
  padding:3px 9px;
  border-radius:999px;
  font-size:12px;
  color:#9da7b3;
  border:1px solid #30363d;
  vertical-align:middle;
}

.subtitle {
  margin-top:8px;
  color:#9da7b3;
  font-size:1.05rem;
}

.actions {
  margin-top:18px;
  display:flex;
  justify-content:center;
  gap:10px;
  flex-wrap:wrap;
}

.btn {
  display:inline-flex;
  align-items:center;
  justify-content:center;
  gap:8px;
  padding:12px 22px;
  border-radius:12px;
  font-weight:800;
  border:1px solid transparent;
  min-height:44px;
}

.btn-primary {
  background:#2da44e;
  color:#ffffff;
}

.btn-primary:hover { filter:brightness(1.08); }

.btn-secondary {
  background:transparent;
  color:#e6edf3;
  border-color:#30363d;
}

.btn-secondary:hover { background:rgba(255,255,255,0.05); }

.lang-switch {
  position:fixed;
  top:14px;
  right:14px;
  z-index:10;
  display:flex;
  gap:8px;
}

.lang-switch button {
  background:rgba(13,17,23,0.75);
  backdrop-filter:blur(8px);
  -webkit-backdrop-filter:blur(8px);
  color:#e6edf3;
  border:1px solid #30363d;
  border-radius:12px;
  padding:8px 12px;
  cursor:pointer;
  min-height:40px;
  font-weight:800;
}

.lang-switch button.active {
  border-color:#58a6ff;
  color:#58a6ff;
  box-shadow:0 0 0 3px rgba(88,166,255,0.12);
}

.section {
  background:rgba(255,255,255,0.03);
  border:1px solid #30363d;
  border-radius:16px;
  padding:18px 20px;
  margin-top:16px;
}

.section h2 {
  margin:0 0 10px;
  color:#f0f6fc;
  font-size:1.25rem;
}

ul { padding-left:18px; margin:10px 0 0; }
li { margin:6px 0; }

.small {
  color:#9da7b3;
  font-size:13px;
  line-height:1.45;
}

.footer {
  margin-top:28px;
  text-align:center;
  color:#9da7b3;
  font-size:14px;
}

/* 📱 Mobile */
@media (max-width:520px) {
  .wrap { padding:22px 12px 56px; }
  .hero h1 { font-size:1.65rem; }
  .btn { width:100%; max-width:360px; }
}
</style>

<div class="lang-switch">
  <button id="btn-de" class="active" onclick="setLang('de', true)">DE</button>
  <button id="btn-en" onclick="setLang('en', true)">EN</button>
</div>

<div class="wrap">

<div class="header">
  <img src="icon.png" alt="Ecowitt MenuBar App Icon" class="app-icon">
</div>

<div class="hero">
  <h1>🌦 Ecowitt MenuBar <span class="badge">Beta</span></h1>

  <div class="subtitle lang-de">
    Schlanke macOS-Menüleisten-App für deine Ecowitt-Wetterstation.
  </div>
  <div class="subtitle lang-en" style="display:none">
    Lightweight macOS menu bar app for your Ecowitt weather station.
  </div>

  <div class="actions">
    <a class="btn btn-primary" href="https://github.com/ecowittApp/ecowitt-App/releases/latest">
      ⬇️ <span class="lang-de">Beta herunterladen</span><span class="lang-en" style="display:none">Download beta</span>
    </a>
    <a class="btn btn-secondary" href="https://github.com/ecowittApp/ecowitt-App/issues">
      🛠 Support
    </a>
  </div>
</div>

<!-- 🔔 UNABHÄNGIGKEITS-HINWEIS -->
<div class="section" style="border-left:4px solid #f0883e;">
  <h2 class="lang-de">ℹ️ Hinweis zur Unabhängigkeit</h2>
  <h2 class="lang-en" style="display:none">ℹ️ Independent project notice</h2>

  <p class="small lang-de">
    Ecowitt MenuBar ist ein unabhängiges Drittanbieter-Softwareprojekt, das von einem einzelnen Entwickler entwickelt wird.<br><br>
    Diese Anwendung ist keine offizielle Ecowitt-App und steht in keiner Verbindung zu Ecowitt, Fine Offset Electronics
    oder verbundenen Unternehmen. Sie wird weder von diesen unterstützt noch empfohlen.<br><br>
    „Ecowitt“ ist eine eingetragene Marke der jeweiligen Rechteinhaber und wird ausschließlich zu beschreibenden Zwecken verwendet.
  </p>

  <p class="small lang-en" style="display:none">
    Ecowitt MenuBar is a third-party, independent software project developed by an individual developer.<br><br>
    This application is not an official Ecowitt app and is not affiliated with, endorsed by, or supported by
    Ecowitt, Fine Offset Electronics, or any related companies.<br><br>
    “Ecowitt” is a registered trademark of its respective owners and is used for descriptive purposes only.
  </p>
</div>

<div class="section">
  <h2 class="lang-de">⭐ Vorteile</h2>
  <h2 class="lang-en" style="display:none">⭐ Benefits</h2>

  <ul class="lang-de">
    <li>Schneller Überblick der wichtigsten Wetterdaten mit nur einem Klick</li>
    <li>Kein aufwendiger Programmaufruf oder Fensterwechsel nötig</li>
    <li>Die relevanten Wetterinformationen jederzeit im Blick</li>
    <li>Ideal für den schnellen Check direkt aus der Menüleiste</li>
  </ul>

  <ul class="lang-en" style="display:none">
    <li>Instant overview of key weather data with a single click</li>
    <li>No need to launch a full application or switch windows</li>
    <li>Essential weather information always visible</li>
    <li>Perfect for quick checks directly from the menu bar</li>
  </ul>
</div>

<div class="section">
  <h2 class="lang-de">✨ Funktionen</h2>
  <h2 class="lang-en" style="display:none">✨ Features</h2>

  <ul class="lang-de">
    <li>Aktuelle Wetterdaten direkt in der macOS-Menüleiste</li>
    <li>Unterstützung für Ecowitt-Wetterstationen</li>
    <li>Automatische Aktualisierung</li>
    <li>Ressourcenschonend &amp; unauffällig</li>
    <li>Optimiert für Dark Mode</li>
  </ul>

  <ul class="lang-en" style="display:none">
    <li>Live weather data directly in the macOS menu bar</li>
    <li>Support for Ecowitt weather stations</li>
    <li>Automatic background updates</li>
    <li>Lightweight and unobtrusive</li>
    <li>Optimized for dark mode</li>
  </ul>
</div>

<div class="section">
  <h2 class="lang-de">🔔 Updates / Neue Versionen</h2>
  <h2 class="lang-en" style="display:none">🔔 Updates / New releases</h2>

  <div class="small lang-de" style="margin-bottom:10px;">
    Neue Versionen werden auf der Projektseite veröffentlicht.
    Wenn du nichts verpassen willst, kannst du das Projekt bei GitHub abonnieren
    oder den Update-Feed nutzen.
  </div>

  <div class="small lang-en" style="display:none; margin-bottom:10px;">
    New versions are published on the project page.
    To get notified, you can follow the project on GitHub
    or subscribe to the update feed.
  </div>

  <div class="small lang-de">
    <strong>Option 1 (GitHub):</strong><br>
    GitHub-Repo öffnen und oben rechts <em>Watch</em> → <em>Custom</em> →
    <em>Releases</em> aktivieren.<br>
    <a href="https://github.com/ecowittApp/ecowitt-App">GitHub-Repo öffnen</a><br><br>

    <strong>Option 2 (RSS-Feed):</strong><br>
    <a href="https://github.com/ecowittApp/ecowitt-App/releases.atom">
      https://github.com/ecowittApp/ecowitt-App/releases.atom
    </a>
  </div>

  <div class="small lang-en" style="display:none">
    <strong>Option 1 (GitHub):</strong><br>
    Open the repository and enable <em>Watch</em> → <em>Custom</em> → <em>Releases</em>.<br>
    <a href="https://github.com/ecowittApp/ecowitt-App">Open GitHub repository</a><br><br>

    <strong>Option 2 (RSS feed):</strong><br>
    <a href="https://github.com/ecowittApp/ecowitt-App/releases.atom">
      https://github.com/ecowittApp/ecowitt-App/releases.atom
    </a>
  </div>
</div>

<div class="footer">
  <div class="lang-de">
    © Christian Henkel (DL7AG) · <a href="https://dl7ag.de">dl7ag.de</a><br>
    Offizielle Projektseite: <strong>https://ecowittapp.dl7ag.de</strong><br>
    <a href="/impressum.html">Impressum</a> · <a href="/datenschutz.html">Datenschutz</a>
    <div class="small" style="margin-top:6px;">
      Diese Website verwendet keine Cookies und kein Tracking.
    </div>
  </div>

  <div class="lang-en" style="display:none">
    © Christian Henkel (DL7AG) · <a href="https://dl7ag.de">dl7ag.de</a><br>
    Official project site: <strong>https://ecowittapp.dl7ag.de</strong><br>
    <a href="/impressum.html">Legal notice</a> · <a href="/privacy.html">Privacy policy</a>
    <div class="small" style="margin-top:6px;">
      This website does not use cookies or tracking.
    </div>
  </div>
</div>

</div>

<script>
(function initLanguage() {
  const stored = localStorage.getItem('lang');
  const browser = (navigator.language || '').toLowerCase().startsWith('de') ? 'de' : 'en';
  setLang(stored || browser, false);
})();

function setLang(lang, persist) {
  document.querySelectorAll('.lang-de').forEach(e => e.style.display = lang === 'de' ? '' : 'none');
  document.querySelectorAll('.lang-en').forEach(e => e.style.display = lang === 'en' ? '' : 'none');
  document.getElementById('btn-de').classList.toggle('active', lang === 'de');
  document.getElementById('btn-en').classList.toggle('active', lang === 'en');
  if (persist) localStorage.setItem('lang', lang);
}
</script>
