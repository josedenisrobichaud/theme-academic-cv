---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "4rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: En résumé (pdf)
        url: uploads/resume_fr.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          #size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: 'Ma recherche'
      subtitle: ''
      text: |-
        Mon objectif est d'explorer l'intersection des enjeux technologiques, sociétaux, environnementaux et climatiques entourant la production laitière afin de soutenir sa durabilité et sa résilience. En m'appuyant sur les bases de l'épidémiologie, je développe des connaissances et des outils liés aux innovations technologiques, aux pratiques de gestion et aux collaborations interdisciplinaires afin d'optimiser la santé des animaux, des producteurs, des consommateurs et de l'environnement.


        N'hésitez pas à me contacter pour collaborer!
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Publications - en vedette
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      fill_image: false
      columns: '2'
  - block: collection
    content:
      title: Publications récentes
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Présentations
      filters:
        folders:
          - event
    design:
      view: article-grid
      fill_image: false
      columns: '2'
  - block: collection
    id: news
    content:
      title: Nouvelles
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
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
      view: title-summary
      # Reduce spacing
      spacing:
        padding: [2rem, 1rem, 2rem, 1rem]

---
