# Steps to build and manage infrastructure

- Review the checklist to ensure the right thing is being built
- Define infrastructure as code
  - Terraform, Packer, Docker
- Build code out of small, standalone, composable modules
- Write automated tests for the modules
- Submit pull requests to trigger code reviews
- Release the new version
- Promote the new version through all environments
  - Local Dev (laptop with Docker)
  - Dev
  - QA / Staging
  - Production