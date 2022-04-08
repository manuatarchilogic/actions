# Actions

## Shared public workflows for Archilogic internal tooling

The purpose of this repository is to house [shared reusable workflows](https://docs.github.com/en/actions/using-workflows/reusing-workflows) that can be used by more than one repository

## Criteria for a new workflow

- Workflow is in use in an existing repository and needed by another repository
- Workflow follows security [best practices](https://docs.github.com/en/github-ae@latest/actions/security-guides/security-hardening-for-github-actions)

## Development

- Workflows should be first developed in the repository they're needed
- Verify internally that the workflow makes sense and copy it to this repository
- Commit changes using semantic commit messages

## Release

Create a release tag via [standard-version](https://github.com/conventional-changelog/standard-version) and push it to origin

```bash
npm run release
```

Don't forget to push the newly created tag to origin

```
git push --follow-tags
```
