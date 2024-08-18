# GOLANG CICD GITHUB
A skeleton repo that has the following component installed for github cicd on golang projects

- `github action` - auto trigger build process
- `goreleaser` - automatically build binaries
- `release please` - formatting
- `conventional commit` - formatting

## Summary
- github action pulls goreleaser to build, build triggered on new tag version
- go releaser references .goreleaser.yaml on how to build
- TODO: use conventional commit and release please 

# Github action
* https://github.com/marketplace/actions/goreleaser-action#run-on-new-tag
* see .github/workflow/release.yaml

# gorelease
* https://goreleaser.com
* you can install locally, but not required if you reuse this repo since the build is done by github action

# Release Please
* https://github.com/googleapis/release-please
* give default github_token permission to create PR
* update github --> repo--> setting --> action general --> workflow permissions --> allow GitHub Actions to create and approve pull request
* need to give the permission in the action yaml
```
permissions:
  contents: write
  pull-requests: write
```

# conventional commit
* https://www.conventionalcommits.org/en/v1.0.0/