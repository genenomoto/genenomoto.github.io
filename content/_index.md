---
# Leave the homepage title empty to use the site title
title: ""
date: 2024-06-08
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: 'Who are you?'
      subtitle: ''
      text: |-
        こんにちは、榎本元と申します。
        東京農業大学　応用生物科学部　農芸化学科　応用微生物学研究室で助教をしています。
        研究の専門は光生物学と微生物学です。酸素発生型光合成を行う原核生物であるシアノバクテリアを主な研究対象にしています。
        光が微生物に当たると何が起きるか、それが微生物の生き様にどのように貢献するのか、その知見をどのように応用できるか、といった研究を展開しています。
        ポスドク期間にドイツでのべ5年過ごした影響で、ドイツ語の勉強も（たまに）続けています。
        研究室参画に興味のある学生さんや研究員の方、共同研究に興味のある研究者/企業の方、お気軽にご連絡ください😃
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: compact
      columns: 1
  - block: collection
    content:
      title: Recent Publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 2
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
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
---
