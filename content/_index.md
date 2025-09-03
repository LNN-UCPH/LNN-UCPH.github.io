---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: hero
    id: about 
    content:
      image:
        filename: lnn-logo.png
      text: |
        <p>
          The Lab for Neuroimaging and Neuroinformatics (LNN) @ UCPH focuses on leveraging advanced imaging technologies and computational methods to study the human brain. We integrate neuroimaging data with neuroinformatics approaches to understand brain structure, function, and connectivity. Our research areas typically include the development and application of machine learning algorithms, image analysis techniques, and data integration methods to advance the field of neuroscience and improve clinical outcomes in neurology and psychiatry. Our work often involves interdisciplinary collaboration, bridging gaps between computational sciences and neuroscience.
        </p>

        <h2>Interests</h2>
        <ul>
          <li>Medical Image Analysis</li>
          <li>Fairness and Bias in Medicine</li>
          <li>Explainable AI</li>
          <li>Neuroinformatics</li>
        </ul>

  - block: people
    id: people
    content:
      title: Meet the Group
      # Choose which groups/teams of users to display.
      #   Edit `user_groups` in each user's profile to add them to one or more of these groups.
      user_groups:
          - Research Scientists
          - Postdoctoral Fellows and PhD students
          - Research Assistants
          - Collaborators
          - Alumni
      sort_by: Params.position
      sort_ascending: true
    design:
      show_interests: true
      show_role: true
      show_social: true

  - block: projects
    id: projects
    content:
      title: Ongoing projects
      sort_by: Params.position
      sort_ascending: true

  - block: collection
    id: publications
    view: citation
    content:
      title: Publications 
      subtitle: ''
      text:
      filters:
        tags: publication
    sort_by: date
    sort_ascending: false
  
---
