---
layout: page
title: Tabs Example
---

# Tabs (No Plugins)

Below is a simple tab implementation using **only HTML + CSS**.

<style>
.tabs {
  display: flex;
  border-bottom: 2px solid #ddd;
  margin-bottom: 1em;
}
.tabs button {
  background: none;
  border: none;
  padding: 0.5em 1em;
  cursor: pointer;
  font-size: 1em;
}
.tabs button.active {
  border-bottom: 2px solid #000;
  font-weight: bold;
}
.tab-content {
  display: none;
}
.tab-content.active {
  display: block;
}
</style>

<div class="tabs">
  <button class="tab-btn active" onclick="openTab(event, 'tab1')">Tab One</button>
  <button class="tab-btn" onclick="openTab(event, 'tab2')">Tab Two</button>
</div>

<div id="tab1" class="tab-content active">
  <p>This is the content of <strong>Tab One</strong>.</p>
</div>

<div id="tab2" class="tab-content">
  <p>This is the content of <strong>Tab Two</strong>.</p>
</div>

<script>
function openTab(evt, tabId) {
  document.querySelectorAll('.tab-content').forEach(el => el.classList.remove('active'));
  document.querySelectorAll('.tab-btn').forEach(el => el.classList.remove('active'));

  document.getElementById(tabId).classList.add('active');
  evt.currentTarget.classList.add('active');
}
</script>
