<style>
:root { color-scheme: dark; }

body {
  background: #0d1117;
  color: #e6edf3;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Inter, Helvetica, Arial, sans-serif;
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
  margin-bottom: 28px;
}

.app-icon {
  width: 96px;
  height: 96px;
  border-radius: 22px;
  box-shadow: 0 12px 30px rgba(0,0,0,.45);
  margin-bottom: 18px;
}

.hero {
  background: rgba(255,255,255,0.03);
  border: 1px solid #30363d;
  border-radius: 18px;
  padding: 28px 22px 26px;
  margin-bottom: 26px;
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
}

.btn {
  display: inline-block;
  padding: 12px 22px;
  border-radius: 12px;
  font-weight: 700;
  border: 1px solid transparent;
  margin: 6px;
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

.btn-secondary:hover {
  background: rgba(255,255,255,0.05);
}

.lang-switch {
  position: fixed;
  top: 16px;
  right: 16px;
  z-index: 10;
}

.lang-switch button {
  background: transparent;
  color: #e6edf3;
  border: 1px solid #30363d;
  border-radius: 10px;
  padding: 6px 12px;
  margin-left: 6px;
  cursor: pointer;
}

.lang-switch button.active {
  border-color: #58a6ff;
  color: #58a6ff;
}

.section {
  background: rgba(255,255,255,0.03);
  border: 1px solid #30363d;
  border-radius: 16px;
  padding: 20px 22px;
  margin-top: 18px;
}

.section h2 {
  margin-top: 0;
  color: #f0f6fc;
}

ul {
  padding-left: 18px;
}

.footer {
  margin-top: 28px;
  text-align: center;
  color: #9da7b3;
  font-size: 14px;
}
</style>

<div class="lang-switch">
  <button id="btn-de" class="active" onclick="setLang('de')">DE</button>
  <button id="btn-en" onclick="setLang('en')">EN</button>
</div>

<div class="wrap">

<div class="header">
  <img src="icon.png" alt="App Icon" class="app-icon">
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
    <li>Ressourcenschonend & unauffällig</li>
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
  <h2>🛠 Support</h2>
  <p>
    <span class="lang-de">Fehler oder Wünsche bitte hier melden:</span>
    <span class="lang-en" style="display:none">Report bugs or feature requests here:</span><br>
    <a href="https://github.com/ecowittApp/ecowitt-App/issues">
      https://github.com/ecowittApp/ecowitt-App/issues
    </a>
  </p>
</div>

<div class="footer">
  <div class="lang-de">
    Entwickelt von Christian Henkel (DL7AG) ·
    <a href="https://dl7ag.de">dl7ag.de</a><br>
    Offizielle Projektseite: <strong>https://ecowittapp.dl7ag.de</strong>
  </div>

  <div class="lang-en" style="display:none">
    Developed by Christian Christian Henkel (DL7AG) ·
    <a href="https://dl7ag.de">dl7ag.de</a><br>
    Official project site: <strong>https://ecowittapp.dl7ag.de</strong>
  </div>
</div>

</div>

<script>
function setLang(lang) {
  document.querySelectorAll('.lang-de').forEach(e => e.style.display = lang === 'de' ? '' : 'none');
  document.querySelectorAll('.lang-en').forEach(e => e.style.display = lang === 'en' ? '' : 'none');
  document.getElementById('btn-de').classList.toggle('active', lang === 'de');
  document.getElementById('btn-en').classList.toggle('active', lang === 'en');
}
</script>
