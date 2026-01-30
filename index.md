<style>
  :root { color-scheme: dark; }

  body {
    background-color: #0d1117;
    color: #e6edf3;
  }

  h1, h2, h3 {
    color: #f0f6fc;
  }

  a {
    color: #58a6ff;
  }

  hr {
    border-color: #30363d;
  }

  .wrap {
    max-width: 920px;
    margin: 0 auto;
    padding: 24px 16px 56px;
  }

  .topbar {
    display:flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 18px;
  }

  .lang button {
    appearance: none;
    border: 1px solid #30363d;
    background: rgba(255,255,255,0.02);
    color: #e6edf3;
    padding: 6px 12px;
    border-radius: 12px;
    font-weight: 700;
    cursor: pointer;
    margin-left: 6px;
  }

  .lang button.active {
    border-color: #58a6ff;
    box-shadow: 0 0 0 3px rgba(88,166,255,0.12);
  }

  .hero {
    padding: 24px 24px 22px;
    border: 1px solid #30363d;
    border-radius: 18px;
    background: rgba(255,255,255,0.02);
    text-align: center;
  }

  .subtitle {
    margin-top: 10px;
    color: #9da7b3;
    font-size: 1.05em;
  }

  .grid {
    display: grid;
    grid-template-columns: 1fr;
    gap: 18px;
    margin-top: 26px;
  }

  .card {
    border: 1px solid #30363d;
    border-radius: 18px;
    padding: 18px 20px;
    background: rgba(255,255,255,0.02);
  }

  .btn {
    display: inline-block;
    padding: 13px 22px;
    border-radius: 14px;
    text-decoration: none;
    font-weight: 700;
    border: 1px solid transparent;
    margin: 14px 8px 0;
  }

  .btn-primary {
    background: #2da44e;
    color: #ffffff;
  }

  .btn-secondary {
    background: transparent;
    color: #e6edf3;
    border-color: #30363d;
  }

  .pill {
    display: inline-block;
    padding: 4px 10px;
    border-radius: 999px;
    border: 1px solid #30363d;
    background: rgba(255,255,255,0.02);
    color: #9da7b3;
    font-size: 13px;
    margin-left: 10px;
  }

  .muted { color: #9da7b3; }

  .lang-de, .lang-en { display:none; }
  .show-de .lang-de { display:block; }
  .show-en .lang-en { display:block; }
</style>

<script>
(function(){
  function setLang(l){
    document.documentElement.classList.remove("show-de","show-en");
    document.documentElement.classList.add(l==="en"?"show-en":"show-de");
    localStorage.setItem("lang",l);
    document.getElementById("btn-de").classList.toggle("active",l==="de");
    document.getElementById("btn-en").classList.toggle("active",l==="en");
  }
  document.addEventListener("DOMContentLoaded",()=>{
    const l=localStorage.getItem("lang")||((navigator.language||"").startsWith("de")?"de":"en");
    setLang(l);
    document.getElementById("btn-de").onclick=()=>setLang("de");
    document.getElementById("btn-en").onclick=()=>setLang("en");
  });
})();
</script>

---
title: Ecowitt MenuBar
---

<div class="wrap">

  <div class="topbar">
    <div class="muted">ecowitt-App</div>
    <div class="lang">
      <button id="btn-de">DE</button>
      <button id="btn-en">EN</button>
    </div>
  </div>

  <p style="text-align:center; margin-bottom:26px;">
    <img src="icon.png" width="128" height="128"
         style="border-radius:24px; box-shadow:0 14px 40px rgba(0,0,0,.65);">
  </p>

  <div class="hero">

    <div class="lang-de">
      <h1>🌦 Ecowitt MenuBar<span class="pill">Beta</span></h1>
      <div class="subtitle">
        Schlanke macOS-Menüleisten-App für deine Ecowitt-Wetterstation.
      </div>

      <a class="btn btn-primary" href="https://github.com/ecowittApp/ecowitt-App/releases/latest">
        ⬇️ Beta herunterladen
      </a>
      <a class="btn btn-secondary" href="https://github.com/ecowittApp/ecowitt-App/issues">
        🛠 Support
      </a>
    </div>

    <div class="lang-en">
      <h1>🌦 Ecowitt MenuBar<span class="pill">Beta</span></h1>
      <div class="subtitle">
        Lightweight macOS menu bar app for your Ecowitt weather station.
      </div>

      <a class="btn btn-primary" href="https://github.com/ecowittApp/ecowitt-App/releases/latest">
        ⬇️ Download beta
      </a>
      <a class="btn btn-secondary" href="https://github.com/ecowittApp/ecowitt-App/issues">
        🛠 Support
      </a>
    </div>

  </div>

  <div class="grid">

    <!-- ADVANTAGES -->
    <div class="card lang-de">
      <h2>⭐ Vorteile</h2>
      <ul>
        <li>Schneller Überblick der wichtigsten Wetterdaten mit nur einem Klick</li>
        <li>Kein aufwendiger Programmaufruf oder Fensterwechsel mehr nötig</li>
        <li>Die relevanten Wetterinformationen jederzeit im Blick</li>
        <li>Ideal für den schnellen Check zwischendurch – direkt aus der Menüleiste</li>
      </ul>
    </div>

    <div class="card lang-en">
      <h2>⭐ Benefits</h2>
      <ul>
        <li>Quick overview of key weather data with a single click</li>
        <li>No need to open a full application or switch windows</li>
        <li>Keep the most important weather information always visible</li>
        <li>Perfect for quick checks directly from the menu bar</li>
      </ul>
    </div>

    <!-- FEATURES -->
    <div class="card lang-de">
      <h2>✨ Funktionen</h2>
      <ul>
        <li>Aktuelle Wetterdaten direkt in der macOS-Menüleiste</li>
        <li>Unterstützung für Ecowitt-Wetterstationen</li>
        <li>Automatische Aktualisierung</li>
        <li>Ressourcenschonend &amp; unauffällig</li>
        <li>Optimiert für Dark Mode</li>
      </ul>
    </div>

    <div class="card lang-en">
      <h2>✨ Features</h2>
      <ul>
        <li>Live weather data directly in the macOS menu bar</li>
        <li>Supports Ecowitt weather stations</li>
        <li>Automatic data refresh</li>
        <li>Lightweight and unobtrusive</li>
        <li>Optimized for dark mode</li>
      </ul>
    </div>

    <!-- SUPPORT -->
    <div class="card lang-de">
      <h2>🛠 Support</h2>
      <p>
        <a href="https://github.com/ecowittApp/ecowitt-App/issues">
          👉 GitHub Issues öffnen
        </a>
      </p>
    </div>

    <div class="card lang-en">
      <h2>🛠 Support</h2>
      <p>
        <a href="https://github.com/ecowittApp/ecowitt-App/issues">
          👉 Open GitHub Issues
        </a>
      </p>
    </div>

  </div>
</div>
