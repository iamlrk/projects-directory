---
# TEMPLATE FOR NEW PROJECTS
# Copy this file, rename it with the next number (e.g., 05-project-name.md)
# Fill in the fields below and delete this comment block

title: Your Project Title
subtitle: Optional subtitle
id: your-project-id  # Use lowercase with hyphens
meta: Tech • Stack • Summary  # Short summary for sidebar
order: 5  # Change this to position in the list
github: https://github.com/username/repo  # Optional
demo: https://your-demo-url.com  # Optional
tech:
  - Technology 1
  - Technology 2
  - Technology 3
  - Add more as needed
---

## Overview

Describe your project here. What does it do? What problem does it solve? Why did you build it?

## Key Features

- Feature 1: Description
- Feature 2: Description
- Feature 3: Description
- Add more features as bullets

## Additional Sections (Optional)

You can add any markdown sections you want:

- Architecture
- Implementation Details
- Challenges
- Future Plans
- Screenshots (using markdown image syntax)

---

## For Project Euler Style Projects (Optional)

If your project has multiple sub-items like Project Euler, add this to frontmatter:

```yaml
euler_problems:  # or rename to match your use case
  - number: 1
    title: Problem Title
    solution: https://link-to-solution
    challenge: What the problem asks
    approach: Your solution strategy
    concepts: Key concepts used
  - number: 2
    title: Another Problem
    # ... etc
```

This will automatically generate:

- A grid index of all items
- Pagination controls
- Detailed views for each item
