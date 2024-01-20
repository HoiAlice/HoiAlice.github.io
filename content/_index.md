---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin

  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: ML Research Scientist
          company: Yandex Research
          company_url: https://research.yandex.com/
          company_logo: yandex
          location: Moscow, Russia
          date_start: '2023-11-14'
          date_end: ''
          description: Working on Large Language Models compression.
        - title: Research Intern
          company: KAUST, Optimization and Machine Learning Lab
          company_url: ''
          company_logo: kaust
          location: Saudi Arabia
          date_start: '2023-07-10'
          date_end: '2023-09-30'
          description: |2-
            * Conducted research under the supervision of _Prof. Peter Richtárik_.
            * Derived theory and ran experiments on distributed optimization, focusing on communication compression.
        - title: ML Engineer Intern (NLP)
          company: Huawei RRI
          company_url: ''
          company_logo: huawei
          location: Moscow, Russia
          date_start: '2022-03-08'
          date_end: '2022-07-05'
          description: |2-
            * Refactored and optimized an _LLM inference framework_ enabling abstract _tabular data_ insertion for efficient _map‑reduce_ inference.
            * Derived theory and ran experiments on distributed optimization, focusing on communication compression.
            * Increased test coverage of the _map‑reduce_ inference interface from 0 to 85% through rigorous unit testing.
            * Took part in developing a _universal LLM benchmarking solution_ adapting _two datasets_ for it.
        - title: Researcher
          company: Terra Quantum AG
          company_url: https://terraquantum.swiss/
          company_logo: tq-black
          location: Moscow, Russia
          date_start: '2019-07-01'
          date_end: '2021-11-01'
          description: |2-
            * Developed a [GRAPE](https://michaelgoerz.net/research/grape_june_2010_slides.pdf) based framework for algorithmic cooling and quantum computations.
            * Investigated the application of tensor networks to combinatorial optimisation.
            * Implemented an amplitude maximum estimation algorithm for pure states via tensor trains.
    design:
      columns: '1'
  - block: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Accomplish&shy;ments'
      subtitle:
      # Date format: https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - date_end: ''
          date_start: '2019-07-16'
          description: Gold Medal
          icon: ipho
          organization: Israel
          title: International Physics Olympiad
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
---
