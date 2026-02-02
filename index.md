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

<!-- 🧾 BETA DISCLAIMER -->
<div class="section" style="border-left:4px solid #d29922;">
  <h2 class="lang-de">🧾 Beta-Haftungsausschluss</h2>
  <h2 class="lang-en" style="display:none">🧾 Beta Disclaimer</h2>

  <p class="small lang-de">
    Diese Software wird als <strong>Beta-Version</strong> bereitgestellt.<br><br>
    Sie kann Fehler, unvollständige Funktionen oder unerwartetes Verhalten enthalten.
    Die Nutzung erfolgt <strong>auf eigene Verantwortung</strong>.<br><br>
    Es wird keine Gewähr für die Richtigkeit, Verfügbarkeit oder Zuverlässigkeit der angezeigten Daten übernommen.
    Der Entwickler übernimmt <strong>keine Haftung für Schäden</strong>, Datenverluste oder Fehlfunktionen,
    die durch die Nutzung dieser Software entstehen.
  </p>

  <p class="small lang-en" style="display:none">
    This software is provided as a <strong>beta version</strong>.<br><br>
    It may contain bugs, incomplete features, or unexpected behavior.
    Use of this software is <strong>at your own risk</strong>.<br><br>
    No guarantee is given for correctness, availability, or reliability of the displayed data.
    The developer assumes <strong>no liability</strong> for any damages, data loss, or malfunctions
    resulting from the use of this software.
  </p>
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

  <div class="small lang-de">
    Neue Versionen werden auf der Projektseite veröffentlicht.<br>
    <a href="https://github.com/ecowittApp/ecowitt-App/releases.atom">
      RSS-Feed abonnieren
    </a>
  </div>

  <div class="small lang-en" style="display:none">
    New versions are published on the project page.<br>
    <a href="https://github.com/ecowittApp/ecowitt-App/releases.atom">
      Subscribe via RSS feed
    </a>
  </div>
</div>

<div class="footer">
  © Christian Henkel (DL7AG) · <a href="https://dl7ag.de">dl7ag.de</a><br>
  <a href="/impressum.html">Impressum</a> · <a href="/datenschutz.html">Datenschutz</a>
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
