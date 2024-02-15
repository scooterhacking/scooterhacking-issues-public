name: SHFW Bug Report
description: Report a bug to help us improve
title: "SHFW BUG: "
labels: ["bug", "shfw"]
body:
  - type: markdown
    attributes:
      value: "Thank you for reporting a bug. Please fill in as much of the template below as you're able."
  - type: input
    id: bug-title
    attributes:
      label: Bug Title
      description: A clear and concise title for the bug.
      placeholder: "Enter a brief title for the bug"
    validations:
      required: true
  - type: textarea
    id: bug-description
    attributes:
      label: Description of the Bug
      description: A detailed description of what the issue is.
      placeholder: "Please describe the issue in as much detail as possible."
    validations:
      required: true
  - type: textarea
    id: steps-to-reproduce
    attributes:
      label: Steps to Reproduce
      description: Please provide the steps to reproduce the issue, if applicable..
      placeholder: |
        1. Go to '...'
        2. Click on '....'
        3. Scroll down to '....'
        4. See error
    validations:
      required: true
  - type: textarea
    id: expected-vs-actual
    attributes:
      label: Expected vs. Actual Behavior
      description: Describe what you expected to happen and what actually happened.
      placeholder: "Expected result... Actual result..."
    validations:
      required: true
  - type: dropdown
    id: environment
    attributes:
      label: Scooter model
      description: Where did the bug occur?
      options:
        - Ninebot G30
        - Ninebot G2
        - Ninebot Es2, Es3, Es4
        - Ninebot E20, E25, E45
        - Xiaomi M365
        - Xiaomi Pro, Pro2, 3
    validations:
      required: true
  - type: input
    id: screenshots
    attributes:
      label: Screenshots
      description: If applicable, add screenshots to help explain your problem.
    validations:
      required: false
  - type: input
    id: contact-info
    attributes:
      label: Contact Information
      description: (Optional) Your discord or telegram username in case we need further details.
      placeholder: "Discord or telegram username"
    validations:
      required: false
