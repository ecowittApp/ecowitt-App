<style>
:root { color-scheme: dark; }

body {
  background: #0d1117;
  color: #e6edf3;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Inter, Helvetica, Arial, sans-serif;
  margin: 0;
}

a { color: #58a6ff; text-decoration: none; }
a:hover { text-decoration: underline; }

.wrap {
  max-width: 920px;
  margin: 0 auto;
  padding: 32px 16px 64px;
}

.header {
  text-align: center;
  margin-bottom: 20px;
}

.app-icon {
  width: 96px;
  height: 96px;
  border-radius: 22px;
  box-shadow: 0 12px 30px rgba(0,0,0,.45);
  margin-bottom: 14px;
}

.hero {
  background: rgba(255,255,255,0.03);
  border: 1px solid #30363d;
  border-radius: 18px;
  padding: 28px 22px 26px;
  margin-bottom: 22px;
  text-align: center;
}

.hero h1 {
  margin: 0 0 6px;
  font-size: 2.1rem;
  color: #f0f6fc;
}

.badge {
  display: inline-block;
  margin-left: 8px;
  padding: 3px 9px;
  border-radius: 999px;
  font-size: 12px;
  color: #9da7b3;
  border: 1px solid #30363d;
  vertical-align: middle;
}

.subtitle {
  margin-top: 8px;
  color: #9da7b3;
  font-size: 1.05rem;
}

.actions {
  margin-top: 18px;
  display: flex;
  justify-content: center;
  gap: 10px;
  flex-wrap: wrap;
}

.btn {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 8px;
  padding: 12px 22px;
  border-radius: 12px;
  font-weight: 800;
  border: 1px solid transparent;
  margin: 0;
  min-height: 44px; /* mobile-friendly tap target */
}

.btn-primary {
  background: #2da44e;
  color: #ffffff;
}

.btn-primary:hover { filter: brightness(1.08); }

.btn-secondary {
  background: transparent;
  color: #e6edf3;
  border-color: #30363d;
}

.btn-secondary:hover { background: rgba(255,255,255,0.05); }

.lang-switch {
  position: fixed;
  top: 14px;
  right: 14px;
  z-index: 10;
  display: flex;
  gap: 8px;
}

.lang-switch button {
  background: rgba(13,17,23,0.75);
  backdrop-filter: blur(8px);
  -webkit-backdrop-filter: blur(8px);
  color: #e6edf3;
  border: 1px solid #30363d;
  border-radius: 12px;
  padding: 8px 12px;
  cursor: pointer;
  min-height: 40px;
  font-weight: 800;
}

.lang-switch button.active {
  border-color: #58a6ff;
  color: #58a6ff;
  box-shadow: 0 0 0 3px rgba(88,166,255,0.12);
}

.section {
  background: rgba(255,255,255,0.03);
  border: 1px solid #30363d;
  border-radius: 16px;
  padding: 18px 20px;
  margin-top: 16px;
}

.section h2 {
  margin: 0 0 10px;
  color: #f0f6fc;
  font-size: 1.25rem;
}

ul { padding-left: 18px; margin: 10px 0 0; }
li { margin: 6px 0; }

.small {
  color: #9da7b3;
  font-size: 13px;
  line-height: 1.45;
}

.kbd {
  font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", "Courier New", monospace;
  font-size: 12px;
  padding: 2px 6px;
  border: 1px solid #30363d;
  border-radius: 8px;
  background: rgba(255,255,255,0.03);
  color: #e6edf3;
}

.footer {
  margin-top: 22px;
  text-align: center;
  color: #9da7b3;
  font-size: 14px;
}

/* 📱 Mobile-Feinschliff */
@media (max-width: 520px) {
  .wrap { padding: 22px 12px 56px; }
  .app-icon { width: 88px; height: 88px; border-radius: 20px; }
  .hero { padding: 22px 16px 20px; border-radius: 16px; }
  .hero h1 { font-size: 1.65rem; line-height: 1.15; }
  .badge { margin-left: 6px; }
  .subtitle { font-size: 1rem; }
  .section { padding: 16px 16px; border-radius: 14px; }
  .section h2 { font-size: 1.15rem; }
  .btn { width: 100%; max-width: 360px; }
  .lang-switch { top: 10px; right: 10px; }
  .lang-switch button { padding: 8px 10px; border-radius: 12px; }
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

  <div class="small" style="margin-top:12px;">
    <span class="lang-de">Tipp: Sprache umschalten oben rechts (DE/EN).</span>
    <span class="lang-en" style="display:none">Tip: Switch language in the top-right corner (DE/EN).</span>
  </div>
</div>

<div class="section">
  <h2 class="lang-de">⭐ Vorteile</h2>
  <h2 class="lang-en" style="display:none">⭐ Benefits</h2>

  <ul class="lang-de">
    <li>Schneller Überblick der wichtigsten Wetterdaten mit nur einem Klick</li>
    <li>Kein aufwendiger Programmaufruf oder Fensterwechsel mehr nötig</li>
    <li>Die relevanten Wetterinformationen jederzeit im Blick</li>
    <li>Ideal für den schnellen Check zwischendurch – direkt aus der Menüleiste</li>
  </ul>

  <ul class="lang-en" style="display:none">
    <li>Instant overview of key weather data with a single click</li>
    <li>No need to launch a full app or switch windows</li>
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
    <li>Automatic background refresh</li>
    <li>Lightweight &amp; unobtrusive</li>
    <li>Optimized for dark mode</li>
  </ul>
</div>

<div class="section">
  <h2>🛠 Support</h2>
  <p class="small" style="margin:0;">
    <span class="lang-de">Fehler oder Wünsche bitte hier melden:</span>
    <span class="lang-en" style="display:none">Report bugs or feature requests here:</span><br>
    <a href="https://github.com/ecowittApp/ecowitt-App/issues">https://github.com/ecowittApp/ecowitt-App/issues</a>
  </p>
</div>

<div class="section">
  <h2 class="lang-de">⚖️ Hinweis / Disclaimer</h2>
  <h2 class="lang-en" style="display:none">⚖️ Disclaimer</h2>

  <div class="small lang-de">
    Dies ist eine inoffizielle, unabhängige Beta-Software. Keine Gewährleistung für Richtigkeit, Verfügbarkeit oder Datenverlust. Nutzung auf eigene Verantwortung.<br>
    „Ecowitt“ ist eine Marke der jeweiligen Rechteinhaber. Dieses Projekt steht in keiner offiziellen Verbindung zu Ecowitt.
  </div>

  <div class="small lang-en" style="display:none">
    This is unofficial, independent beta software. No warranty for accuracy, availability, or data loss. Use at your own risk.<br>
    “Ecowitt” is a trademark of its respective owners. This project is not affiliated with Ecowitt.
  </div>
</div>

<div class="footer">
  <div class="lang-de">
    Entwickelt von Christian Henkel (DL7AG) · <a href="https://dl7ag.de">dl7ag.de</a><br>
    Offizielle Projektseite: <strong>https://ecowittapp.dl7ag.de</strong>
  </div>

  <div class="lang-en" style="display:none">
    Developed by Christian Henkel (DL7AG) · <a href="https://dl7ag.de">dl7ag.de</a><br>
    Official project site: <strong>https://ecowittapp.dl7ag.de</strong>
  </div>
</div>

</div>

<script>
(function initLanguage() {
  // 🌍 automatische Spracherkennung (Browser-Language), aber User-Wahl gewinnt
  const stored = localStorage.getItem('lang');
  const browser = (navigator.language || '').toLowerCase().startsWith('de') ? 'de' : 'en';
  const initial = stored || browser;
  setLang(initial, false);
})();

function setLang(lang, persist) {
  document.querySelectorAll('.lang-de').forEach(e => e.style.display = (lang === 'de') ? '' : 'none');
  document.querySelectorAll('.lang-en').forEach(e => e.style.display = (lang === 'en') ? '' : 'none');
  document.getElementById('btn-de').classList.toggle('active', lang === 'de');
  document.getElementById('btn-en').classList.toggle('active', lang === 'en');
  if (persist) localStorage.setItem('lang', lang);
}
</script>
