---
#widget: podcasts
#headless: true
weight: 70

title: Recent & Current Podcasts
subtitle: Episodes That Inspire and Inform Me

#draft: false
#type: widget # Ensure your theme supports custom sections
---

<section id="recent-podcasts">
  <h2>Recent Podcasts</h2>
  <ul>
    {{ range first 3 (where .Site.Pages "Section" "podcasts" | sort "Date" "desc") }}
      <li>
        <h3>{{ .Title }}</h3>
        <p>{{ .Params.description }}</p>
        <p><em>{{ .Date.Format "Jan 2, 2006" }}</em></p>
      </li>
    {{ end }}
  </ul>
  <a href="/podcasts/">See All Episodes</a>
</section>