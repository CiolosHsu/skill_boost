name: Skill Boost Task
description: Daily skill boost checklist item
title: "Day X: [Task Title]"
labels: ["skill-boost"]
assignees: ["CiolosHsu"]

body:
  - type: markdown
    attributes:
      value: |
        ## 🎯 Learning Goal
        Describe what you want to achieve today.

  - type: input
    id: task
    attributes:
      label: Task
      description: What is the specific task for today?
      placeholder: e.g. Learn JOIN and CTE

  - type: textarea
    id: resources
    attributes:
      label: Resources
      description: Links, docs, or datasets you will use.
      placeholder: e.g. Kaggle dataset, PostgreSQL docs

  - type: textarea
    id: deliverables
    attributes:
      label: Deliverables
      description: What should be uploaded or demonstrated?
      placeholder: e.g. SQL script, ETL pipeline demo

  - type: checkboxes
    id: status
    attributes:
      label: Status
      options:
        - label: Completed
