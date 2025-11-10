---
# Leave the homepage title empty to use the site title
title: "Home"
date: 2022-11-02
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3 
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: fiona
      text: ''
      # Show a call-to-action button under your biography? (optional)
      # button:
        #text: Download CV
        #url: uploads/resume.pdf
      headings:
        about: 'About'
        education: 'Services'
        interests: 'Specialisms'
    design:
      # Apply a gradient background
      css_class: hbx-bg-gradient
      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: rounded # Options: circle (default), square, rounded
  - block: collection
    id: events
    content:
      title: Events
      filters:
        folders:
          - events
      count: 6
    design:
      view: article-grid
      columns: 3
  - block: collection
    id: blog
    content:
      title: Blog
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: blog
      # Choose how many pages you would like to display (0 = all pages)
      count: 4
      # Filter on criteria
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: article-grid 
      columns: 2
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0] 
  - block: markdown
    id: contact
    content:
      title: Contact
      text: 
        Drop me a message at <a href="mailto:hello@fionamacneill.co.uk">hello@fionamacneill.co.uk</a>
    design:
      columns: '1'
---
