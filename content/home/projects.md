---
# An instance of the Portfolio widget.
# Documentation: https://wowchemy.com/docs/page-builder/
widget: portfolio
active: true
# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 30

title: Projects
subtitle: ''

# <p>Hi</p>


content:
  
  
  # Page type to display. E.g. project.
  page_type: project

  # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
  filter_default: 0

  # Filter toolbar (optional).
  # Add or remove as many filters (`filter_button` instances) as you like.
  # To show all items, set `tag` to "*".
  # To filter by a specific tag, set `tag` to an existing tag name.
  # To remove the toolbar, delete the entire `filter_button` block.
  filter_button:
  - name: All
    tag: '*'
  - name: Privacy-Preserving and Robust Machine Learning at the Edge
    tag: 'Privacy-Preserving and Robust Machine Learning at the Edge'
  - name: Efficient Large-Scale Distributed Learning in the Cloud
    tag: 'Efficient Large-Scale Distributed Learning in the Cloud'
  - name: Foundations of Coded Computing
    tag: 'Foundations of Coded Computing'
  - name: Other
    tag: 'Other'

design:
  # Choose how many columns the section has. Valid values: '1' or '2'.
  columns: '1'

  # Toggle between the various page layout types.
  #   1 = List
  #   2 = Compact
  #   3 = Card
  #   5 = Showcase
  view: 3

  # For Showcase view, flip alternate rows?
  flip_alt_rows: false
---
