# Template repo for Go SDK  
This template helps developers get started with the Go SDK and initiate indexing process on pkg.go.dev repository

## Contents
This repository contains the following:

- A `README` that contains the instructions
- A GitHub Action workflow to initiate publishing the Go SDK to [pkg.go.dev](https://pkg.go.dev/) package repository (as suggested in the [official publishing tutorial](https://go.dev/doc/modules/publishing)).


## Instructions

1. Create a new target Go SDK Repo by clicking the **Use this template** button at the top of this repository.

2. Run the GitHub Action `Generate SDKs using liblab` in the Control Repo that builds the SDK, and raises a PR against this target SDK Repo.

3. Review and merge the PR.

4. Create a release with a tag in the target SDK Repo.

5. The GitHub Action `Publish to pkg.go.dev` in the target SDK Repo initiates the indexing proces

6. After the time needed for the indexing process to be finished (tipically around 30 minutes or less), package should be accessible at `https://pkg.go.dev/github.com/{go-module-name}@{tag}`
