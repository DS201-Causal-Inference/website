---
layout: home
title: 🏠 Home
nav_order: 1
---

# Causal Inference
{: .mb-2 }
DS-UA 201 · Spring 2027 · New York University
{: .fs-6 .fw-300 }

**Lecture:** Wednesdays, 4:55–7:25 p.m. · Washington Square · Room TBA  
**Instructors:** [Nishant Kheterpal](https://nishant.page) and [Lucius Bynum](https://luciusbynum.com/)  
**Laboratories:** Fridays · [See sections and times](./staff/#laboratory-sections)

{: .note }
> This site is in preparation. The schedule, assessments, and policies are tentative and may change.

<div class="reading-font-control">
  <label for="reading-font">Reading font</label>
  <select id="reading-font">
    <option value="default">Default</option>
    <option value="palatino">Palatino</option>
    <option value="atkinson">Atkinson Hyperlegible Next</option>
  </select>
</div>
<script>
(function () {
  var select = document.getElementById('reading-font');
  try { select.value = localStorage.getItem('ds201-reading-font') || 'default'; } catch (_) {}
  select.addEventListener('change', function () {
    document.documentElement.classList.remove('font-palatino', 'font-atkinson');
    if (select.value !== 'default') document.documentElement.classList.add('font-' + select.value);
    try { localStorage.setItem('ds201-reading-font', select.value); } catch (_) {}
  });
})();
</script>

## About the course

Causal inference provides tools for understanding cause and effect. We begin with experiments and the design of data collection, then study what it means to make a causal claim and how to evaluate threats to validity. We will explore experiments and methods for observational data, including quasi-experiments, regression discontinuity, difference in differences, and contemporary approaches. Lectures develop the conceptual and statistical foundations; laboratories explore implementation in Python.

## Course schedule

The topics below are a working plan. Lecture notes, lab materials, and assignment links will appear as they become available.

{% for module in site.modules %}
{{ module }}
{% endfor %}

The midterm placement is a tentative planning estimate. The final exam takes place during the university exam period; its date and time are TBA. [NYU academic calendar](https://bulletins.nyu.edu/nyu/academic-calendar/).
