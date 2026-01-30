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
    gap: 12px;
    margin-bottom: 18px;
  }

  .lang {
    display:flex;
    gap: 8px;
    align-items: center;
  }

  .lang button {
    appearance: none;
    border: 1px solid #30363d;
    background: rgba(255,255,255,0.02);
    color: #e6edf3;
    padding: 8px 12px;
    border-radius: 12px;
    font-weight: 700;
    cursor: pointer;
  }

  .lang button:hover {
    background: rgba(255,255,255,0.05);
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

  .btn-primary:hover {
    filter: brightness(1.08);
  }

  .btn-secondary {
    background: transparent;
    color: #e6edf3;
    border-color: #30363d;
  }

  .btn-secondary:hover {
    background: rgba(255,255,255,0.05);
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
    vertical-align: middle;
  }

  .muted {
    color: #9da7b3;
  }

  /* Language visibility */
  .lang-de, .lang-en { display: none; }
  .show-de .lang-de { display: block; }
  .show-en .lang-en { display: block; }
</style>

<script>
  (function () {
    function setLang(lang) {
      var root = document.documentElement;
      root.classList.remove("show-de", "show-en");
      root.classList.add(lang === "en" ? "show-en" : "show-de");

      var deBtn = document.getElementById("btn-de");
      var enBtn = document.getElementById("btn-en");
      if (deBtn && enBtn) {
        deBtn.classList.toggle("active", lang !== "en");
        enBtn.classList.toggle("active", lang === "en");
      }

      try { localStorage.setItem("ecowitt_lang", lang); } catch (e) {}
    }

    function detect() {
      var saved = null;
      try { saved = localStorage.getItem("ecowitt_lang"); } catch (e) {}
      if (saved === "de" || saved === "en") return saved;

      var nav = (navigator.language || "").toLowerCase();
      return nav.startsWith("de") ? "de" : "en";
    }

    window.ecowittSetLang = setLang;

    document.addEventListener("DOMContentLoaded", function () {
      setLang(detect());
      var deBtn = document.getElementById("btn-de");
      var enBtn = document.getElementById("btn-en");
      if (deBtn) deBtn.addEventListener("click", function(){ setLang("de"); });
      if (enBtn) enBtn.addEventListener("click", function(){ setLang("en"); });
    });
  })();
</script>

---
title: Ecowitt MenuBar
---

<div class="wrap">

  <div class="topbar">
    <div class="muted">ecowitt-App</div>
    <div class="lang" aria-label="Language switch">
      <button id="btn-de" type="button">DE</button>
      <button id="btn-en" type="button">EN</button>
    </div>
  </div>

  <p style="text-align:center; margin-bottom:26px;">
    <img src="icon.png"
         alt="Ecowitt MenuBar App Icon"
         width="128"
         height="128"
         style="
           border-radius:24px;
           box-shadow: 0 14px 40px rgba(0,0,0,0.65);
         ">
  </p>

  <div class="hero">

    <div class="lang-de">
      <h1>🌦 Ecowitt MenuBar (macOS)<span class="pill">Beta</span></h1>
      <div class="subtitle">
        Schlanke macOS-Menüleisten-App zur Anzeige deiner Ecowitt-Wetterstation.
      </div>

      <div style="margin-top:6px;">
        <a class="btn btn-primary"
           href="https://github.com/ecowittApp/ecowitt-App/releases/latest">
          ⬇️ Aktuelle Beta herunterladen
        </a>

        <a class="btn btn-secondary"
           href="https://github.com/ecowittApp/ecowitt-App/issues">
          🛠 Support / Issues
        </a>
      </div>

      <div class="muted" style="margin-top:16px;">
        Hinweis: Beim ersten Start ggf. unter<br>
        <b>Systemeinstellungen → Datenschutz &amp; Sicherheit</b>
        die App explizit erlauben.
      </div>
    </div>

    <div class="lang-en">
      <h1>🌦 Ecowitt MenuBar (macOS)<span class="pill">Beta</span></h1>
      <div class="subtitle">
        Lightweight macOS menu bar app to display your Ecowitt weather station data.
      </div>

      <div style="margin-top:6px;">
        <a class="btn btn-primary"
           href="https://github.com/ecowittApp/ecowitt-App/releases/latest">
          ⬇️ Download latest beta
        </a>

        <a class="btn btn-secondary"
           href="https://github.com/ecowittApp/ecowitt-App/issues">
          🛠 Support / Issues
        </a>
      </div>

      <div class="muted" style="margin-top:16px;">
        Note: On first launch, you may need to allow the app in<br>
        <b>System Settings → Privacy &amp; Security</b>.
      </div>
    </div>

  </div>

  <div class="grid">

    <div class="card lang-de">
      <h2>🧪 Beta-Status</h2>
      <p>
        Diese Version ist eine öffentliche Beta.
        Feedback und Bugreports sind ausdrücklich erwünscht.
      </p>
      <p class="muted">
        Bitte bei Meldungen macOS-Version, App-Version und
        idealerweise einen Screenshot angeben.
      </p>
    </div>

    <div class="card lang-en">
      <h2>🧪 Beta status</h2>
      <p>
        This is a public beta release. Feedback and bug reports are very welcome.
      </p>
      <p class="muted">
        Please include your macOS version, app version, and ideally a screenshot.
      </p>
    </div>

    <div class="card lang-de">
      <h2>🖥 Voraussetzungen</h2>
      <ul>
        <li>macOS 13 oder neuer</li>
        <li>Ecowitt API-Key</li>
      </ul>
    </div>

    <div class="card lang-en">
      <h2>🖥 Requirements</h2>
      <ul>
        <li>macOS 13 or later</li>
        <li>Ecowitt API key</li>
      </ul>
    </div>

    <div class="card lang-de">
      <h2>🛠 Support</h2>
      <p>Fehler oder Wünsche bitte als Issue melden:</p>
      <p>
        <a href="https://github.com/ecowittApp/ecowitt-App/issues">
          👉 https://github.com/ecowittApp/ecowitt-App/issues
        </a>
      </p>
    </div>

    <div class="card lang-en">
      <h2>🛠 Support</h2>
      <p>Please report bugs or feature requests as an issue:</p>
      <p>
        <a href="https://github.com/ecowittApp/ecowitt-App/issues">
          👉 https://github.com/ecowittApp/ecowitt-App/issues
        </a>
      </p>
    </div>

    <div class="card lang-de">
      <h2>👤 Entwickler</h2>
      <p>
        <b>Christian Henkel (DL7AG)</b><br>
        <a href="https://dl7ag.de">👉 https://dl7ag.de</a>
      </p>
    </div>

    <div class="card lang-en">
      <h2>👤 Developer</h2>
      <p>
        <b>Christian Henkel (DL7AG)</b><br>
        <a href="https://dl7ag.de">👉 https://dl7ag.de</a>
      </p>
    </div>

  </div>
</div>
