---
#widget: podcasts
#headless: true
weight: 70

title: Recent & Current Podcasts
subtitle: Episodes That Inspire and Inform Me
content:
  # Page type to display. E.g. project.
  page_type: podcasts
#draft: false
#type: widget # Ensure your theme supports custom sections
design:
  columns: '2'
---

{{ define "main" }}
<div class="podcasts-section">
  <h2>Latest Podcasts</h2>
  <ul class="podcasts-list">
    {{ range .Pages }}
    <li>
      <div class="podcast-icon">{{ .Params.icon }}</div>
      <div>
        <a href="{{ .Params.link }}" class="podcast-title" target="_blank">{{ .Title }}</a>
        <p class="podcast-description">{{ .Params.description }}</p>
      </div>
    </li>
    {{ end }}
  </ul>
</div>
{{ end }}