---
layout: page
title: Tabs Example
---

# Tabs (No Plugins)

Below is a simple tab implementation using **only HTML + CSS**.

<style>
/* ===== Tabs ===== */
.tabs-wrapper {
  margin-top: 1rem;
}

.tabs {
  display: flex;
  gap: 0.5rem;
  overflow-x: auto;
  -webkit-overflow-scrolling: touch;
  border-bottom: 2px solid #e5e5e5;
  padding-bottom: 0.25rem;
}

.tabs::-webkit-scrollbar { display: none; }
.tabs { scrollbar-width: none; }

.tab-btn {
  flex: 0 0 auto;
  background: #f5f5f5;
  border: none;
  border-radius: 999px;
  padding: 0.65rem 1.2rem;
  font-size: 0.95rem;
  cursor: pointer;
  white-space: nowrap;
}

.tab-btn.active {
  background: #000;
  color: #fff;
}

.tab-content {
  display: none;
  padding-top: 1rem;
}

.tab-content.active {
  display: block;
}

/* ===== Collapsible / FAQ ===== */
details {
  border: 1px solid #ddd;
  border-radius: 6px;
  padding: 0.75rem 1rem;
  margin-bottom: 0.75rem;
  background: #fafafa;
}

summary {
  cursor: pointer;
  font-weight: 600;
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

/* Desktop tweak */
@media (min-width: 640px) {
  .tab-btn { border-radius: 6px; }
}
</style>

<div class="tabs-wrapper">
  <div class="tabs">
    <button class="tab-btn active" onclick="openTab(event, 'overview')">Overview</button>
    <button class="tab-btn" onclick="openTab(event, 'guidelines')">Guidelines</button>
    <button class="tab-btn" onclick="openTab(event, 'steps')">Step-by-Step</button>
    <button class="tab-btn" onclick="openTab(event, 'examples')">Examples</button>
  </div>

  <!-- OVERVIEW -->
  <div id="overview" class="tab-content active">

    <h3>Why am I doing this?</h3>
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

    <h3>Why is the reward $10?</h3>
    <ul>
      <li>I handle official filing and taxes</li>
      <li>Official rewards take 1+ year — you get paid immediately</li>
      <li>Many offenders never pay, meaning I get $0</li>
      <li>I shield you from bureaucracy and risk</li>
    </ul>

    <p>
      Filming <strong>5–10 incidents per day</strong> is realistic for someone already on NYC streets.
    </p>
    <p>
      That’s <strong>$50–$100 per day</strong> extra.
    </p>

  </div>

  <!-- GUIDELINES -->
  <div id="guidelines" class="tab-content">

    <details open>
      <summary>Principles</summary>
      <ul>
        <li>Only commercial vehicles and buses</li>
        <li>No private vehicles, Ubers, taxis, city or police vehicles</li>
        <li>Vehicle must not move for <strong>3:10 minutes</strong></li>
        <li>Audible engine noise or visible exhaust required</li>
        <li>No mitigating factors may occur</li>
        <li>License plate and DOT # must be clearly visible</li>
      </ul>
    </details>

    <details>
      <summary>Mitigating Factors</summary>
      <ul>
        <li><strong>Trucks:</strong> tail lift, cooling unit, secondary engine</li>
        <li>
          <strong>Buses:</strong> no passengers entering/exiting, no luggage loading
          <br>
          (entire right side must be visible)
        </li>
        <li><strong>Vans/Pickups:</strong> no commercial plate, cooling unit</li>
      </ul>
    </details>

  </div>

  <!-- STEPS -->
  <div id="steps" class="tab-content">

    <ol>
      <li>
        Download a timestamp + location video app:
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

  </div>

  <!-- EXAMPLES -->
  <div id="examples" class="tab-content">

    <h3>Photo Examples</h3>
    <p>(Replace these placeholders with real screenshots)</p>

    <div class="example-grid">
      <img src="https://via.placeholder.com/300x200?text=License+Plate+Visible" alt="">
      <img src="https://via.placeholder.com/300x200?text=Exhaust+Visible" alt="">
      <img src="https://via.placeholder.com/300x200?text=Bus+Right+Side" alt="">
    </div>

  </div>
</div>

<script>
function openTab(evt, tabId) {
  document.querySelectorAll('.tab-content').forEach(el => el.classList.remove('active'));
  document.querySelectorAll('.tab-btn').forEach(el => el.classList.remove('active'));

  document.getElementById(tabId).classList.add('active');
  evt.currentTarget.classList.add('active');

  history.replaceState(null, '', '#' + tabId);
  localStorage.setItem('activeTab', tabId);
}

// Restore tab from URL or storage
(function () {
  const hash = location.hash.replace('#', '');
  const saved = localStorage.getItem('activeTab');
  const tab = hash || saved;
  if (tab && document.getElementById(tab)) {
    document.querySelector(`.tab-btn[onclick*="${tab}"]`)?.click();
  }
})();
</script>
