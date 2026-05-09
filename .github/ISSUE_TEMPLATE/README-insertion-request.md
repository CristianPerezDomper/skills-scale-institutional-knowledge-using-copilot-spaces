---
name: "Add Content to Project Management Process Docs"
description: "Request to add new content or updates to an existing program management process document."
title: "[Process Doc Update]: README, project management processes summary, and links for OctoAcme Project Management Docs"
labels: ["documentation", "process improvement"]
body:
  - type: dropdown
    id: process_doc
    attributes:
      label: "Which process document do you want to update? (If this is a new document, select '')"
      description: "Select the program management process document you want to add content to. If this is a new process doc, choose ''."
      options:
        - octoacme-project-management-overview.md
        - octoacme-project-initiation.md
        - octoacme-project-planning.md
        - octoacme-execution-and-tracking.md
        - octoacme-risks-and-communication.md
        - octoacme-release-and-deployment.md
        - octoacme-retrospective-and-continuous-improvement.md
        - octoacme-roles-and-personas.md
        - 
    validations:
      required: true

  - type: textarea
    id: content_summary
    attributes:
      label: "Summary of New Content"
      description: "Briefly describe the new content or update you want to add."
      placeholder: "E.g., Add clarification to risk escalation paths, new checklist for releases, additional role responsibilities, etc."
    validations:
      required: true

  - type: textarea
    id: rationale
    attributes:
      label: "Why is this update needed?"
      description: "Explain the reason for this addition. Is it to address a gap, improve clarity, incorporate a best practice, etc.?"
      placeholder: "E.g., Identified gap in process, team feedback, alignment with industry standards, etc."
    validations:
      required: true

  - type: textarea
    id: example_content
    attributes:
      label: "Suggested Content (optional)"
      description: "Paste the proposed new text, checklist, diagram, or example content you'd like to add. (Optional)"
      placeholder: "E.g., - New checklist items, - Copy for a new section, - Example scenario, etc."

  - type: checkboxes
    id: acceptance_criteria
    attributes:
      label: "Acceptance Criteria"
      description: "Check all that apply:"
      options:
        - label: "Content aligns with existing process docs"
        - label: "Update improves clarity or closes a documented gap"
        - label: "Proposed content has been reviewed with stakeholders (if needed)"
---

### Which process document do you want to update?
<new document>

### Summary of New Content
Create a README in the `docs` folder that provides:
- A brief summary describing the project management processes used by OctoAcme (overview-style).
- A linked list to all process documentation files currently in `docs/`, making navigation and discovery easier for new and current team members.

### Why is this update needed?
The README will serve as a central entry point for the OctoAcme project management documentation, making it faster to onboard new team members and easier for anyone to find key process docs. This addresses the need for discoverability, transparency, and quick reference as described in our Copilot Space goals.

### Suggested Content (optional):
````markdown
# OctoAcme Project Management Docs

Welcome! This folder contains the core project management processes and templates used by OctoAcme teams.

## Project Management Process Summary
OctoAcme manages projects using a lightweight, iterative approach focused on customer value, cross-functional alignment, clear roles, and measurable outcomes. Processes cover the full project lifecycle: initiation, planning, execution/tracking, risk management, release, and retrospectives. See links below for process details and templates.

## Process Documents
- [Project Management Overview](./octoacme-project-management-overview.md)
- [Project Initiation Guide](./octoacme-project-initiation.md)
- [Project Planning](./octoacme-project-planning.md)
- [Execution & Tracking](./octoacme-execution-and-tracking.md)
- [Risk Management & Communication](./octoacme-risks-and-communication.md)
- [Release & Deployment Guide](./octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)
- [Roles and Personas](./octoacme-roles-and-personas.md)
````

### Acceptance Criteria
- [x] Content aligns with existing process docs
- [x] Update improves clarity or closes a documented gap
- [ ] Proposed content has been reviewed with stakeholders (if needed)
