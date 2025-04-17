---
title: Home
layout: home
nav_order: 1
---

# Preprint Review Metadata Modelling

## 🤔 What am I looking at?
This documentation provides examples of how and where Preprint Review Metadata is currently deposited and how to retrieve and  share it. It is organised as fields that are inputs to or outputs from the process. 


Each element is categorised as "essential" or "desirable" to the process and accompanied by a health score that is determined by the number of preprint peer-review initiatives sharing this information and the places in which it can be recorded.

🔴 =  Not well captured or well implemented immediate community action needed, 

🟡 = partially collected/implemented, observe whether further community action needed, 

🟢 = well collected and implemented, 

grey = no further action required at this stage.

## Contributors

<div class="contributors">
{% for contributor in site.github.contributors %}
  <div class="contributor">
    <a href="https://github.com/{{ contributor.login }}" target="_blank" rel="noopener noreferrer">
      <img src="{{ contributor.avatar_url }}" alt="{{ contributor.login }}" width="50" height="50" class="contributor-avatar">
      <span class="contributor-name">{{ contributor.login }}</span>
    </a>
  </div>
{% endfor %}
</div>
