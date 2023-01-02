---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
      text:
  - block: features
    content:
      title: Skills
      items:
        - name: R
          description: ''
          icon: r-project
          icon_pack: fab
        - name: Statistics
          description: ''
          icon: chart-line
          icon_pack: fas
        - name: Python
          descriptio: ''
          icon: python
          icon_pack: fab
  - block: experience
    content:
      title: Formação Acadêmica 
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Bacharelado em Estatística
          company: Universidade Federal do Paraná
          company_url: ''
          location: Curitiba / PR
          date_start: '2020-01-01'
          date_end: ''
        - title: Técnico em Administração
          company: Escola Técnica de Registro - Centro Paula Souza
          company_url: ''
          location: Registro / SP
          date_start: '2014-01-01'
          date_end: '2015-07-31'
    design:
      columns: '2'
  - block: experience
    content:
      title: Experiência Profissional
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Estágio - Departamento de Recuperação de Crédito
          company: Bradesco
          company_url: ''
          location: Curitiba / PR
          date_start: '2022-12-21'
          date_end: ''
        - title:  Bolsista - PET Estatística
          company: Universidade Federal do Paraná
          company_url: ''
          location: Curitiba / PR
          date_start: '2022-07-01'
          date_end: ''
        - title: Estágio - Núcleo de Estatística e Monitoramento da Corregedoria
          company: Tribunal de Justiça do Estado do Paraná
          company_url: ''
          location: Curitiba / PR
          date_start: '2022-07-01'
          date_end: '2022-12-13'
          description: |2-
              Responsibilities include:

              * Analysing
              * Modelling
              * Deploying
    design:
      columns: '2'
  - block: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Certificados'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: https://lms.ev.org.br/mpls/Web/Lms/Student/PrintCertificateDialog.aspx?CpSFAULT79H5WmkxifukpKfLfNtl3%2fRr
          date_end: ''
          date_start: '2022-11-11'
          description: ''
          organization: Fundação Bradesco
          organization_url: https://www.ev.org.br/
          title: Linguagem de Programação Python - Básico
          url: 'https://www.ev.org.br/'
        - certificate_url: https://lms.ev.org.br/mpls/Web/Lms/Student/PrintCertificateDialog.aspx?CpSFAULT79H5WmkxifukpKfLfNtl3%2fRr
          date_end: ''
          date_start: '2021-01-01'
          description: Formulated informed blockchain models, hypotheses, and use cases.
          organization: Fundação Bradesco
          organization_url: https://www.ev.org.br/
          title: Linguagem de Programação Python - Básico
          url: https://www.edx.org/professional-certificate/uc-berkeleyx-blockchain-fundamentals
        - certificate_url: https://www.datacamp.com
          date_end: '2020-12-21'
          date_start: '2020-07-01'
          description: ''
          organization: DataCamp
          organization_url: https://www.datacamp.com
          title: 'Object-Oriented Programming in R'
          url: ''
    design:
      columns: '2'
  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
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
      view: compact
      columns: '2'
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: Deep Learning
          tag: Deep Learning
        - name: Other
          tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Qualquer dúvida ou comentário fique à vontade.
      # Contact (add or remove contact options as necessary)
      email: dennyandrew@ufpr.br
      phone: (41) 99837-4848
      contact_links:
        - icon: linkedin
          icon_pack: fab
          name: LinkedIn
          link: 'https://www.linkedin.com/in/denny-andrew-137598160/'
        - icon: instagram
          icon_pack: fab
          name: Instagram
          link: 'https://www.instagram.com/denny_andrew/'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---
