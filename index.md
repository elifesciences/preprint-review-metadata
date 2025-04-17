---
title: Home
layout: home
nav_order: 1
---

# Preprint Review Metadata Modelling
[![DOI](https://zenodo.org/badge/956511465.svg)](https://doi.org/10.5281/zenodo.15236642)

## 🤔 What am I looking at?
This documentation provides examples of how and where Preprint Review Metadata is currently deposited and how to retrieve and  share it. It is organised as fields that are inputs to or outputs from the process. 

Each element is categorised as "essential" or "desirable" to the process and accompanied by a health score that is determined by the number of preprint peer-review initiatives sharing this information and the places in which it can be recorded.

🔴 =  Not well captured or well implemented immediate community action needed, 

🟡 = partially collected/implemented, observe whether further community action needed, 

🟢 = well collected and implemented, 

grey = no further action required at this stage.

Each page contains an actions/updates section where members of the community can discuss actions that could be taken to improve the deposit and retrieval of the metadata.

Contributors are encouraged to make edits to the pages.

## Contributors

<div id="contributors" class="contributors"></div>

<script>
  fetch('https://api.github.com/repos/elifesciences/preprint-review-metadata/contributors')
    .then(res => res.json())
    .then(data => {
      const container = document.getElementById('contributors');
      data.forEach(contributor => {
        const div = document.createElement('div');
        div.className = 'contributor';
        div.innerHTML = `
          <a href="${contributor.html_url}" target="_blank" rel="noopener noreferrer">
            <img src="${contributor.avatar_url}" alt="${contributor.login}" width="50" height="50" class="contributor-avatar" style="border-radius: 50%;">
            <span class="contributor-name">${contributor.login}</span>
          </a>
        `;
        container.appendChild(div);
      });
    });
</script>
