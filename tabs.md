---
layout: page
title: Tabs Example
---

# Tabs (No Plugins)

Below is a simple tab implementation using **only HTML + CSS**.

<style>
/* Container */
.tabs-wrapper {
  margin-top: 1rem;
}

/* Tabs row */
.tabs {
  display: flex;
  gap: 0.5rem;
  overflow-x: auto;
  -webkit-overflow-scrolling: touch;
  border-bottom: 2px solid #e5e5e5;
  padding-bottom: 0.25rem;
}

/* Hide scrollbar (mobile-friendly) */
.tabs::-webkit-scrollbar {
  display: none;
}
.tabs {
  scrollbar-width: none;
}

/* Tab buttons */
.tab-btn {
  flex: 0 0 auto;
  background: #f5f5f5;
  border: none;
  border-radius: 999px;
  padding: 0.5rem 1rem;
  font-size: 0.95rem;
  cursor: pointer;
  white-space: nowrap;
}

/* Active tab */
.tab-btn.active {
  background: #000;
  color: #fff;
}

/* Content */
.tab-content {
  display: none;
  padding-top: 1rem;
}

.tab-content.active {
  display: block;
}

/* Desktop enhancement */
@media (min-width: 640px) {
  .tabs {
    border-bottom: none;
  }
  .tab-btn {
    border-radius: 6px;
  }
}
</style>

<div class="tabs-wrapper">
  <div class="tabs">
    <button class="tab-btn active" onclick="openTab(event, 'tab1')">Overview</button>
    <button class="tab-btn" onclick="openTab(event, 'tab2')">Details</button>
    <button class="tab-btn" onclick="openTab(event, 'tab3')">Examples</button>
  </div>

  <div id="tab1" class="tab-content active">
    <p>This is the <strong>Overview</strong> tab.</p>
  </div>

  <div id="tab2" class="tab-content">
    <p>This is the <strong>Details</strong> tab.</p>
  </div>

  <div id="tab3" class="tab-content">
    <p>This is the <strong>Examples</strong> tab.</p>
  </div>
</div>

<script>
function openTab(evt, tabId) {
  evt.currentTarget
    .closest('.tabs-wrapper')
    .querySelectorAll('.tab-content')
    .forEach(el => el.classList.remove('active'));

  evt.currentTarget
    .closest('.tabs')
    .querySelectorAll('.tab-btn')
    .forEach(el => el.classList.remove('active'));

  document.getElementById(tabId).classList.add('active');
  evt.currentTarget.classList.add('active');
}
</script>
