---
# Leave the homepage title empty to use the site title
title: "Home"
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: fiona
      text: ""
      # Show a call-to-action button under your biography? (optional)
      #button:
      #  text: Download CV
      #  url: uploads/resume.pdf
    design:
      css_class: dark
      #background:
        #color: 
        #image:
          # Add your image background to `assets/media/`.
          #filename: stacked-peaks.svg
          #filters:
          #  brightness: 1.0
          #size: cover
          #position: center
          #parallax: false

  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 3 
       # Reduce spacing
      spacing:
        padding: [4rem, 0, 0, 0]
  - block: collection
    id: projects
    content:
      title: Portfolio 
      filters:
        folders:
          - project
        featured_only: false 
    design:
      view: article-grid
      columns: 3 
      # Reduce spacing
      spacing:
        padding: [0, 0, 4rem, 0]
  - block: collection
    id: blog
    content:
      title: Blog
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 8
      # Filter on criteria
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: article-grid 
      columns: 4
      # Reduce spacing
      spacing:
        padding: [0, 0, 4rem, 0]
  - block: markdown
    id: contact
    content:
      title: 'Contact'
      subtitle: ''
      text: |-
        <div style="text-align:center;"> 
        <a href="mailto:hello@fionamacneill.co.uk">hello@fionamacneill.co.uk</a>
        <p>Macknowlogist Ltd. <br>83 Queens Road <br>Brighton <br>BN1 3XE</p> 
        <strong>Company number:</strong> 16146243
        </div>
    design:
      columns: '1'
      spacing:
        padding: [0, 0, 0, 0]
---
