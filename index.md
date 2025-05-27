---
layout: default
---

{% include_relative README.md %}

---

## [Introduction](#){: .section-title onclick="toggleSection('introduction')" }
<div id="introduction" class="section-content" style="display: none;">
{% include_relative 01_Introduction/README.md %}
</div>

---

## [Single Responsibility](#){: .section-title onclick="toggleSection('single-responsibility')" }
<div id="single-responsibility" class="section-content" style="display: none;">
{% include_relative 02_Single_Responsibility/README.md %}
</div>

--

<div class="section-container">
  <h2 class="section-title" onclick="toggleSection('single-responsibility')">Single Responsibility Principle</h2>
  <div id="single-responsibility" class="section-content" style="display: none;">
    {% include_relative 02_Single_Responsibility/README.md %}
  </div>
</div>

---

<div class="section-container">
  <h2 class="section-title" onclick="toggleSection('open-close')">Open/Close Principle</h2>
  <div id="open-close" class="section-content" style="display: none;">
    {% include_relative 03_Open_Close/README.md %}
  </div>
</div>

---

<div class="section-container">
  <h2 class="section-title" onclick="toggleSection('liskov-substitution')">Liskov Substitution Principle</h2>
  <div id="liskov-substitution" class="section-content" style="display: none;">
    {% include_relative 04_Liskov_Substitution/README.md %}
  </div>
</div>

---

<div class="section-container">
  <h2 class="section-title" onclick="toggleSection('interface-segregation')">Interface Segregation Principle</h2>
  <div id="interface-segregation" class="section-content" style="display: none;">
    {% include_relative 05_Interface_Segregation/README.md %}
  </div>
</div>

---

<div class="section-container">
  <h2 class="section-title" onclick="toggleSection('dependency-inversion')">Dependency Inversion Principle</h2>
  <div id="dependency-inversion" class="section-content" style="display: none;">
    {% include_relative 06_Dependency_Inversion/README.md %}
  </div>
</div>

<script>
function toggleSection(sectionId) {
  const section = document.getElementById(sectionId);
  if (section.style.display === "none") {
    // Hide all sections first
    const allSections = document.getElementsByClassName("section-content");
    for (let i = 0; i < allSections.length; i++) {
      allSections[i].style.display = "none";
    }
    // Show the clicked section
    section.style.display = "block";
  } else {
    section.style.display = "none";
  }
}
</script>

<style>
.section-title {
  cursor: pointer;
  padding: 10px;
  background-color: #f0f0f0;
  border-radius: 5px;
  margin-bottom: 10px;
}

.section-title:hover {
  background-color: #e0e0e0;
}

.section-content {
  padding: 10px;
  border-left: 3px solid #ccc;
  margin-left: 10px;
}
</style>