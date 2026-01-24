---
layout: page
title: Tabs Example
---

# Tabs (No Plugins)

Below is a simple tab implementation using **only HTML + CSS**.

<style>
/* ===== Language Tabs ===== */
.lang-tabs {
  display: flex;
  gap: 0.5rem;
  margin-bottom: 1rem;
  flex-wrap: wrap; /* allows wrapping on small screens */
}

.lang-btn {
  background: #f5f5f5;
  border: none;
  border-radius: 12px;
  padding: 1rem 1.5rem;
  font-size: 1.1rem;
  font-weight: 600;
  cursor: pointer;
  text-align: center;
  flex: 1 1 100%;   /* full width on small screens */
  min-width: 120px;
  transition: background 0.2s;
}

.lang-btn.active {
  background: #000;
  color: #fff;
}

/* For larger screens, make buttons smaller and inline */
@media (min-width: 480px) {
  .lang-btn {
    flex: 1; /* equal width side by side */
  }
}

.lang-content {
  display: none;
}

.lang-content.active {
  display: block;
}

/* ===== TOC ===== */
.toc {
  border: 1px solid #ddd;
  border-radius: 6px;
  padding: 1rem;
  margin: 1.5rem 0;
  background: #fafafa;
}

.toc ul {
  padding-left: 1.25rem;
}

/* ===== Collapsible ===== */
details {
  border: 1px solid #ddd;
  border-radius: 6px;
  padding: 0.75rem 1rem;
  margin-bottom: 0.75rem;
  background: #fafafa;
}

summary {
  font-weight: 600;
  cursor: pointer;
}

/* ===== Images ===== */
.example-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(140px, 1fr));
  gap: 0.75rem;
}

.example-grid img {
  width: 100%;
  border-radius: 6px;
  border: 1px solid #ddd;
}
</style>

<!-- LANGUAGE TABS -->
<div class="lang-tabs">
  <button class="lang-btn active" onclick="switchLang('en')">English</button>
  <button class="lang-btn" onclick="switchLang('es')">Español</button>
</div>

<!-- ================= ENGLISH ================= -->
<div id="lang-en" class="lang-content active">

<h2 id="top">Earn $10 for Recording Idling Vehicles</h2>

<div class="toc">
  <strong>Table of Contents</strong>
  <ul>
    <li><a href="#why">Why am I doing this?</a></li>
    <li><a href="#reward">Why is the reward $10?</a></li>
    <li><a href="#earnings">How much can I earn?</a></li>
    <li><a href="#guidelines">Video guidelines</a></li>
    <li><a href="#steps">Step-by-step</a></li>
    <li><a href="#examples">Examples</a></li>
  </ul>
</div>

<h3 id="why">Why am I doing this?</h3>
<p>
I’ve been recording these videos myself for several years and am making good money.
My reporting process is streamlined and takes very little time.
</p>
<p>
The limiting factor is capturing incidents — which I can crowdsource through you.
</p>

<ul>
  <li>You make easy money</li>
  <li>I make money</li>
  <li>The city gets cleaner air</li>
</ul>

<h3 id="reward">Why is the reward $10?</h3>
<ul>
  <li>I handle filing the complaint and paying taxes</li>
  <li>Official rewards take 1+ year — you get paid immediately</li>
  <li>Many offenders never pay, meaning I get $0</li>
  <li>I shield you from bureaucracy and risk</li>
</ul>

<h3 id="earnings">How much can I earn?</h3>
<p>
For someone already on NYC streets, capturing <strong>5–10 incidents per day</strong> is realistic.
</p>
<p>
That’s <strong>$50–$100 per day</strong>.
</p>

<h3 id="guidelines">Video guidelines</h3>

<details open>
  <summary>Principles</summary>
  <ul>
    <li>Only commercial vehicles and buses</li>
    <li>No private vehicles, Ubers, taxis, city or police vehicles</li>
    <li>Vehicle must not move for <strong>3:10 minutes</strong></li>
    <li>Audible engine noise or visible exhaust required</li>
    <li>License plate and DOT number must be visible</li>
  </ul>
</details>

<details>
  <summary>Mitigating factors</summary>
  <ul>
    <li><strong>Trucks:</strong> tail lift, cooling unit, secondary engine</li>
    <li>
      <strong>Buses:</strong> no passengers or luggage loading
      (entire right side must be visible)
    </li>
    <li><strong>Vans/Pickups:</strong> no commercial plate, cooling unit</li>
  </ul>
</details>

<h3 id="steps">Step-by-step</h3>
<ol>
  <li>
    Download a timestamp + location camera:
    <ul>
      <li>
        <a href="https://play.google.com/store/apps/details?id=com.jeyluta.timestampcamerafreeent&pli=1" target="_blank">
          Android – Timestamp Camera
        </a>
      </li>
      <li>
        <a href="https://apps.apple.com/ph/app/timestamp-camera-enterprise/id1297201432" target="_blank">
          iOS – Timestamp Camera Enterprise
        </a>
      </li>
    </ul>
  </li>
  <li>Record the full video following guidelines</li>
  <li>Rename the file to your <strong>Venmo username</strong></li>
  <li>
    Upload here:
    <a href="https://we.tl/r-nGvpVZiFwo" target="_blank">WeTransfer</a>
  </li>
  <li>Approved videos earn <strong>$10</strong></li>
</ol>

<h3 id="examples">Examples</h3>
<div class="example-grid">
  <img src="https://via.placeholder.com/300x200?text=License+Plate" alt="">
  <img src="https://via.placeholder.com/300x200?text=Exhaust" alt="">
  <img src="https://via.placeholder.com/300x200?text=Bus+Right+Side" alt="">
</div>

</div>

<!-- ================= SPANISH ================= -->
<div id="lang-es" class="lang-content">

<h2 id="top-es">Gana $10 grabando vehículos en ralentí</h2>

<div class="toc">
  <strong>Tabla de Contenidos</strong>
  <ul>
    <li><a href="#why-es">¿Por qué hago esto?</a></li>
    <li><a href="#reward-es">¿Por qué la recompensa es $10?</a></li>
    <li><a href="#earnings-es">¿Cuánto puedo ganar?</a></li>
    <li><a href="#guidelines-es">Guías de video</a></li>
    <li><a href="#steps-es">Paso a paso</a></li>
    <li><a href="#examples-es">Ejemplos</a></li>
  </ul>
</div>

<h3 id="why-es">¿Por qué hago esto?</h3>
<p>
He estado grabando estos videos yo mismo durante varios años y he estado ganando buen dinero.
Mi proceso de reportes está optimizado y ahora toma muy poco tiempo.
</p>
<p>
El factor limitante es capturar incidentes, lo que puedo hacer mediante crowdsourcing contigo.
</p>

<ul>
  <li>Tú ganas dinero fácilmente</li>
  <li>Yo gano dinero</li>
  <li>La ciudad obtiene aire más limpio</li>
</ul>

<h3 id="reward-es">¿Por qué la recompensa es $10?</h3>
<ul>
  <li>Yo me encargo de presentar la queja y pagar impuestos</li>
  <li>Las recompensas oficiales tardan más de un año — tú recibes dinero de inmediato</li>
  <li>Muchos infractores nunca pagan, lo que significa que yo recibo $0</li>
  <li>Te protejo de la burocracia y el riesgo</li>
</ul>

<h3 id="earnings-es">¿Cuánto puedo ganar?</h3>
<p>
Para alguien que ya pasa tiempo en las calles de NYC, capturar <strong>5–10 incidentes por día</strong> es realista.
</p>
<p>
Eso significa <strong>$50–$100 diarios</strong>.
</p>

<h3 id="guidelines-es">Guías de video</h3>

<details open>
  <summary>Principios</summary>
  <ul>
    <li>Solo vehículos comerciales y autobuses</li>
    <li>No vehículos privados, Ubers, taxis, vehículos de la ciudad o policía</li>
    <li>El vehículo no debe moverse durante <strong>3:10 minutos</strong></li>
    <li>Se requiere ruido de motor audible o humo visible</li>
    <li>La matrícula y número DOT deben ser visibles</li>
  </ul>
</details>

<details>
  <summary>Factores atenuantes</summary>
  <ul>
    <li><strong>Camiones:</strong> uso de elevador de cola, unidad de refrigeración, motor secundario</li>
    <li>
      <strong>Autobuses:</strong> sin pasajeros subiendo/bajando, sin carga de equipaje
      (todo el lado derecho debe ser visible)
    </li>
    <li><strong>Furgonetas / pickups:</strong> sin placa comercial, unidad de refrigeración</li>
  </ul>
</details>

<h3 id="steps-es">Paso a paso</h3>
<ol>
  <li>
    Descarga una cámara que agregue fecha, hora y ubicación:
    <ul>
      <li>
        <a href="https://play.google.com/store/apps/details?id=com.jeyluta.timestampcamerafreeent&pli=1" target="_blank">
          Android – Timestamp Camera
        </a>
      </li>
      <li>
        <a href="https://apps.apple.com/ph/app/timestamp-camera-enterprise/id1297201432" target="_blank">
          iOS – Timestamp Camera Enterprise
        </a>
      </li>
    </ul>
  </li>
  <li>Graba el video completo siguiendo las guías</li>
  <li>Renombra el archivo con tu <strong>usuario de Venmo</strong></li>
  <li>
    Sube el video aquí:
    <a href="https://we.tl/r-nGvpVZiFwo" target="_blank">WeTransfer</a>
  </li>
  <li>Videos aprobados ganan <strong>$10</strong></li>
</ol>

<h3 id="examples-es">Ejemplos</h3>
<div class="example-grid">
  <img src="https://via.placeholder.com/300x200?text=Matrícula+Visible" alt="">
  <img src="https://via.placeholder.com/300x200?text=Humo+Visible" alt="">
  <img src="https://via.placeholder.com/300x200?text=Lado+Derecho+Autobús" alt="">
</div>

</div>

<script>
function switchLang(lang) {
  document.querySelectorAll('.lang-content').forEach(el => el.classList.remove('active'));
  document.querySelectorAll('.lang-btn').forEach(el => el.classList.remove('active'));

  document.getElementById('lang-' + lang).classList.add('active');
  document.querySelector(`[onclick="switchLang('${lang}')"]`).classList.add('active');

  localStorage.setItem('lang', lang);
}

// Restore language
(function () {
  const saved = localStorage.getItem('lang');
  if (saved) switchLang(saved);
})();
</script>
