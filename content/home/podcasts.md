---
# Documentation: https://wowchemy.com/docs/page-builder/
widget: pages  # Use the pages widget
headless: true  # This ensures it's part of the home page
weight: 70

title: Recent & Current Podcasts
subtitle: Episodes That Inspire and Inform Me

content:
  # Page type to display. E.g. post, talk, publication...
  page_type: podcasts
  # Choose how many pages you would like to display (0 = all pages)
  count: 3
  # Choose how many pages you would like to offset by
  offset: 0
  # Page order: descending (desc) or ascending (asc) date.
  order: desc
  # Filter on criteria
  filters:
    folders:
      - podcasts
    tag: ''
    category: ''
    publication_type: ''
    author: ''
    exclude_featured: false
    exclude_future: false
    exclude_past: false

design:
  # Choose how many columns the section has. Valid values: '1' or '2'.
  columns: '1'
  # Toggle between the various page layout types.
  #   1 = List
  #   2 = Compact
  #   3 = Card
  #   4 = Citation (publication only)
  view: 2
---