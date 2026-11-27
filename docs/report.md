# Lab 7 Report: Git, GitHub and CI/CD

## Objective
To use Git for version control, create a CI pipeline with GitHub Actions, and understand deployment and rollback.

## Tools
Git, GitHub, GitHub Codespaces, GitHub Actions, Docker.

## Resources
- GitHub repository: systems-network-admin-lab
- app/index.html (web page)
- docker/Dockerfile (nginx image)
- .github/workflows/ci.yml (CI pipeline)

## Git workflow
I created a repository, committed the initial files, created a feature branch (feature/update-page), changed the page from Version 1 to Version 2, pushed it, opened a pull request and merged it after the CI check passed.

## CI vs CD
CI (Continuous Integration) means every code change is automatically built and tested. CD (Continuous Deployment) means code that passes the tests is automatically released to a server.

## Pipeline stages
1. Checkout code
2. Validate files
3. Build Docker image
4. Run container and test with curl

## Purpose of code review and version history
A pull request lets another person review changes before they reach main. Version history records who changed what and when, so mistakes can be traced.

## Rollback
If a release breaks, use git revert to undo the bad commit, or redeploy the previous working Docker image tag.

## Terraform
Not included in this assignment.

## Conclusion
I learned how Git branches, pull requests and automated CI checks help deliver code safely.