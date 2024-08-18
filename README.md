# GOLANG CICD GITHUB
A skeleton repo that has the following component installed for github cicd on golang projects

- `github action` - auto trigger build process
- `goreleaser` - automatically build binaries
- `release please` - formatting
- `conventional commit` - formatting

# Github action
* https://github.com/marketplace/actions/goreleaser-action#run-on-new-tag
* see .github/workflow/release.yaml

# gorelease
* https://goreleaser.com
* you can install locally, but not required if you reuse this repo since the build is done by github action

# Release Please
* https://github.com/googleapis/release-please

# conventional commit
* https://www.conventionalcommits.org/en/v1.0.0/