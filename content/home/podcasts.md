---
widget: tag_cloud
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
  css_style: 'podcast_css' 
---


<div class="podcasts-section">
  <h2>Podcasts</h2>
  <ul>
    {{ range .Pages }}
    <li>
      <h3><a href="{{ .Params.link }}" target="_blank">{{ .Title }}</a></h3>
      <p>{{ .Params.description }}</p>
      <p><strong>Date:</strong> {{ .Date.Format "Jan 2, 2006" }}</p>
    </li>
    {{ end }}
  </ul>
</div>
