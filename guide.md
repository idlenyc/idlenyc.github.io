---
layout: default
title: Guide
---

# Guide on producing idle videos

<style>
/* ===== Language Tabs ===== */
.lang-tabs {
  display: flex;
  gap: 0.75rem;
  margin-bottom: 1.25rem;
  flex-wrap: wrap;
}

.lang-btn {
  background: #f5f5f5;
  border: none;
  border-radius: 14px;
  padding: 1.1rem 1.5rem;
  font-size: 1.15rem;
  font-weight: 600;
  cursor: pointer;
  text-align: center;
  flex: 1 1 100%;
}

.lang-btn.active {
  background: #000;
  color: #fff;
}

@media (min-width: 480px) {
  .lang-btn {
    flex: 1;
  }
}

/* ===== Language Visibility ===== */
.lang-content {
  display: none;
}

.lang-content.active {
  display: block;
}

/* ===== Collapsible Sections ===== */
details.content-section {
  border: 1px solid #ddd;
  border-radius: 10px;
  padding: 0.85rem 1.1rem;
  margin-bottom: 1rem;
  background: #fafafa;
}

details.content-section summary {
  font-weight: 700;
  cursor: pointer;
  font-size: 1.1rem;
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

/* ===== Intro Box ===== */
.intro-box {
  background: #f0f8ff;
  border-left: 5px solid #007700;
  border-radius: 10px;
  padding: 1.25rem 1.5rem;
  margin-bottom: 1rem;
}

.intro-box h2 {
  margin-top: 0;
  font-size: 1.45rem;
  font-weight: 700;
}

.intro-box p {
  font-size: 1.1rem;
  line-height: 1.5;
}

/* ===== Sticky Upload Link ===== */
.sticky-upload {
  position: sticky;
  top: 0.75rem;
  background: #fff;
  z-index: 1000;
  padding: 0.75rem 0;
  margin-bottom: 1rem;
  display: flex;
  justify-content: center;
}

.upload-link {
  display: inline-block;
  background-color: #28a745;
  color: #fff !important;
  padding: 0.85rem 1.25rem;
  border-radius: 12px;
  font-weight: 600;
  text-decoration: none;
  font-size: 1.15rem;
}

.upload-link:hover {
  background-color: #218838;
}

/* ===== CTA Box ===== */
.cta-box {
  border: 2px solid #28a745; /* subtle green for action */
  border-radius: 14px;
  padding: 1.25rem 1.4rem;
  margin: 1.5rem 0;
  background: #fff;
}

.cta-box h3 {
  margin-top: 0;
  font-size: 1.3rem;
}

.cta-box ul {
  margin-left: 1.2rem;
}

.cta-box strong {
  font-weight: 700;
}

/* ===== Emoji accents in headings ===== */
.intro-box h2::before,
.cta-box h3::before {
  content: "📹 ";
  margin-right: 0.25rem;
}

.cta-box h3::before {
  content: "💰 ";
}
</style>

<!-- LANGUAGE TABS -->
<div class="lang-tabs">
  <button class="lang-btn active" onclick="switchLang('en')">English</button>
  <button class="lang-btn" onclick="switchLang('es')">Español</button>
</div>

<!-- ================= ENGLISH ================= -->
<div id="lang-en" class="lang-content active">

<div class="intro-box">
  <h2>Earn Extra Cash in NYC – It’s Easy!</h2>
  <p>Spot idling commercial vehicles or buses, record a short video, and get $10 for each qualifying submission.  
  No sign-up, no waiting, just quick, simple rewards for helping keep NYC air cleaner.</p>
</div>

<!-- Sticky upload link -->
<div class="sticky-upload">
  <a href="https://we.tl/r-nGvpVZiFwo" target="_blank" class="upload-link">Upload Your Video Here</a>
</div>

<details class="content-section">
  <summary>Why am I doing this?</summary>
  <p>I have been recording these videos myself for several years and am making good money.</p>
  <p>My reporting process is streamlined and does not take much time.</p>
  <p>The limiting factor is capturing incidents, which I can crowdsource through you.</p>
  <ul>
    <li>You make easy money</li>
    <li>I make money</li>
    <li>The city gets cleaner air</li>
  </ul>
</details>

<details class="content-section">
  <summary>Why is the reward $10?</summary>
  <ul>
    <li>I officially file the complaint and pay all taxes</li>
    <li>Getting the official reward takes at least one year</li>
    <li>You get paid immediately</li>
    <li>Often the offender does not pay at all, so I get $0</li>
    <li>I shield you from the complicated process and long wait</li>
  </ul>
</details>

<details class="content-section">
  <summary>How much can I earn?</summary>
  <p>For someone already spending time on the streets of NYC, capturing <strong>5–10 incidents per day</strong> is realistic.</p>
  <p><strong>$50–$100 per day</strong></p>
</details>

<details class="content-section">
  <summary>What are the guidelines for a successful video?</summary>

  <h4>Principles</h4>
  <ul>
    <li>Only commercial vehicles and buses</li>
    <li>No private vehicles, Ubers, taxis, city vehicles or police cars</li>
    <li>Vehicle must not move for <strong>3:10 minutes</strong></li>
    <li>Audible engine noise or visible exhaust plume required</li>
    <li>License plate and DOT number must be clearly visible</li>
  </ul>

  <h4>Mitigating Factors</h4>
  <ul>
    <li><strong>Truck:</strong> tail lift, cooling unit, secondary engine</li>
    <li><strong>Bus:</strong> no passengers entering/exiting, no luggage loading (entire right side must be filmed)</li>
    <li><strong>Vans / Pickups:</strong> no commercial plate, cooling unit</li>
  </ul>
</details>

<details class="content-section">
  <summary>Step-by-step guide</summary>
  <ol>
    <li>
      Download a video app that adds timestamps and location:
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
    <li>Record the full video following the guidelines</li>
    <li>Rename the file to your <strong>Venmo username</strong></li>
    <li>Upload it using the link above</li>
    <li>If approved, you receive <strong>$10</strong></li>
  </ol>
</details>

<details class="content-section">
  <summary>Examples</summary>
  <div class="example-grid">
    <img src="https://via.placeholder.com/300x200?text=License+Plate+Visible" alt="">
    <img src="https://via.placeholder.com/300x200?text=Visible+Exhaust" alt="">
    <img src="https://via.placeholder.com/300x200?text=Bus+Right+Side" alt="">
  </div>
</details>

<!-- CTA Box -->
<div class="cta-box">
  <h3>Ready to get started?</h3>
  <p>If you’re already spending time on the streets of NYC, recording idling vehicles can be an easy way to earn extra cash.  
  All you need is your phone and a few minutes per incident.</p>
  <ul>
    <li>Record a qualifying video</li>
    <li>Rename it to your Venmo username</li>
    <li>Upload it using the link above</li>
    <li><strong>Get paid $10 if approved</strong></li>
  </ul>
  <p><strong>No sign-up. No paperwork. No waiting.</strong></p>
</div>

<details class="content-section">
  <summary>Legal Disclaimer</summary>
  <p>By submitting a video, you confirm that you recorded it legally, from a public place, without trespassing, and in compliance with all applicable laws.</p>
  <p>You are not an employee, contractor, or agent of the website operator. Participation is voluntary.</p>
  <p>Payment is offered as a goodwill reward for usable footage and is not guaranteed.</p>
</details>

</div>

<!-- ================= SPANISH ================= -->
<div id="lang-es" class="lang-content">

<div class="intro-box">
  <h2>Gana dinero extra en NYC – ¡Es fácil!</h2>
  <p>Identifica vehículos comerciales o autobuses en ralentí, graba un breve video y recibe $10 por cada envío válido.  
  Sin registro, sin esperas, solo recompensas rápidas por ayudar a mantener el aire de NYC más limpio.</p>
</div>

<!-- Sticky upload link -->
<div class="sticky-upload">
  <a href="https://we.tl/r-nGvpVZiFwo" target="_blank" class="upload-link">Sube tu video aquí</a>
</div>

<details class="content-section">
  <summary>¿Por qué hago esto?</summary>
  <p>He estado grabando estos videos yo mismo durante varios años y he generado buenos ingresos.</p>
  <p>Mi proceso de reporte está optimizado y ahora toma muy poco tiempo.</p>
  <p>El factor limitante es capturar los incidentes, algo que puedo externalizar contigo.</p>
  <ul>
    <li>Tú ganas dinero fácilmente</li>
    <li>Yo gano dinero</li>
    <li>La ciudad obtiene aire más limpio</li>
  </ul>
</details>

<details class="content-section">
  <summary>¿Por qué la recompensa es $10?</summary>
  <ul>
    <li>Yo me encargo de presentar la denuncia oficialmente y pagar los impuestos</li>
    <li>Las recompensas oficiales tardan al menos un año, muchas veces más</li>
    <li>Tú recibes el dinero de inmediato</li>
    <li>En muchos casos el infractor nunca paga y yo recibo $0</li>
    <li>Te protejo del proceso complicado y de la larga espera</li>
  </ul>
</details>

<details class="content-section">
  <summary>¿Cuánto puedo ganar?</summary>
  <p>Para alguien que ya pasa tiempo en las calles de NYC, capturar entre <strong>5 y 10 incidentes por día</strong> es totalmente posible.</p>
  <p><strong>$50–$100 dólares por día</strong></p>
</details>

<details class="content-section">
  <summary>¿Cuáles son las guías para un video válido?</summary>

  <h4>Principios</h4>
  <ul>
    <li>Solo se pueden reportar vehículos comerciales y autobuses</li>
    <li>No vehículos privados, Ubers, taxis, vehículos de la ciudad ni policías</li>
    <li>El vehículo no debe moverse durante <strong>3:10 minutos</strong></li>
    <li>Debe escucharse el motor o verse claramente el humo del escape</li>
    <li>La matrícula y el número DOT deben verse claramente</li>
  </ul>

  <h4>Factores atenuantes</h4>
  <ul>
    <li><strong>Camiones:</strong> plataforma elevadora, unidad de refrigeración, motor secundario</li>
    <li><strong>Autobuses:</strong> sin subida/bajada de pasajeros ni carga de equipaje (se debe grabar todo el lado derecho)</li>
    <li><strong>Vans / Pickups:</strong> sin placa comercial, unidad de refrigeración</li>
  </ul>
</details>

<details class="content-section">
  <summary>Guía paso a paso</summary>
  <ol>
    <li>
      Descarga una aplicación de video que agregue fecha, hora y ubicación:
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
    <li>Graba el video completo cumpliendo las guías</li>
    <li>Cambia el nombre del archivo a tu <strong>usuario de Venmo</strong></li>
    <li>Súbelo usando el enlace arriba</li>
    <li>Si el video es aprobado, recibes <strong>$10</strong></li>
  </ol>
</details>

<details class="content-section">
  <summary>Ejemplos</summary>
  <div class="example-grid">
    <img src="https://via.placeholder.com/300x200?text=Matrícula+Visible" alt="">
    <img src="https://via.placeholder.com/300x200?text=Humo+Visible" alt="">
    <img src="https://via.placeholder.com/300x200?text=Lado+Derecho+Autobús" alt="">
  </div>
</details>

<!-- CTA Box -->
<div class="cta-box">
  <h3>¿Listo para empezar?</h3>
  <p>Si ya pasas tiempo en las calles de NYC, grabar vehículos en ralentí puede ser una forma sencilla de ganar dinero extra.  
  Solo necesitas tu teléfono y unos minutos por incidente.</p>
  <ul>
    <li>Graba un video válido</li>
    <li>Cámbiale el nombre a tu usuario de Venmo</li>
    <li>Súbelo usando el enlace arriba</li>
    <li><strong>Recibe $10 si es aprobado</strong></li>
  </ul>
  <p><strong>Sin registro. Sin papeleo. Sin esperas.</strong></p>
</div>

<details class="content-section">
  <summary>Aviso Legal</summary>
  <p>Esta página es solo para fines informativos y no constituye asesoramiento legal.</p>
  <p>Al enviar un video, confirmas que fue grabado legalmente, desde un lugar público, sin invadir propiedad privada y cumpliendo todas las leyes aplicables.</p>
  <p>No eres empleado, contratista ni representante del operador del sitio. La participación es voluntaria.</p>
  <p>El pago se ofrece como una recompensa de buena fe por material utilizable y no está garantizado.</p>
  <p>El operador del sitio es el único responsable de presentar denuncias oficiales y no asume responsabilidad por problemas derivados de la grabación o el envío.</p>
</details>

</div>

<script>
function switchLang(lang) {
  document.querySelectorAll('.lang-content').forEach(el => el.classList.remove('active'));
  document.querySelectorAll('.lang-btn').forEach(el => el.classList.remove('active'));
  document.getElementById('lang-' + lang).classList.add('active');
  document.querySelector(`[onclick="switchLang('${lang}')"]`).classList.add('active');
}
</script>
