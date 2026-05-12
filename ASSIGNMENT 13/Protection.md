# Branch Protection Rules

Branch protection rules were configured for the main branch to improve code quality and maintain repository stability.

## Rules Applied

### Require Pull Request Reviews
At least one reviewer must approve changes before merging into main.

### Require Status Checks
The CI workflow must pass successfully before pull requests can be merged.

### Disable Direct Pushes
Developers cannot push directly to main. All changes must go through pull requests.

---

# Why These Rules Matter

## Improved Code Quality
Code reviews help identify bugs and improve maintainability.

## Prevent Broken Code
Automated tests ensure failing code cannot be merged.

## Team Collaboration
Pull requests encourage communication and structured development workflows.

## Industry Best Practice
Branch protection and CI/CD pipelines are standard practices used in modern software development.
