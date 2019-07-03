## Overview:

This issue is intended to document for our current processes within this project.

## Contents:

- [Linting](#Linting)
- [Git Branching Model](#Git-branching-model)
- [Naming Branches](#Naming-Branches)
- [Commit messages](#Commit-Messages)
- [Pull Request Checklist](#Pull-Request-Checklist)
- [Merging Pull Requests](#Merging-Pull-Requests)

## Linting

- To begin with, we would suggest using eslint with the airbnb style guide configuration for easy setup (to be done on one computer and added to project file)
- Further edits to the linter configuration file can be discussed, agreed on, and documented here.

## Git Branching Model

![image alt](https://nvie.com/img/git-model@2x.png)

Further informations in this artical here : https://nvie.com/posts/a-successful-git-branching-model/
## Naming Branches

- feature/fix convention
  - E.g. `feature/add-search-function` , `test/add-search-function` or `fix/change-searchbar-color`

## Commit Messages

- Should include issue #
- Written with 'imperative tone' to describe what a commit does, rather than what it did.
  - E.g. `Change color of search bar` instead of `Changed/changes color of search bar`



## Pre Pull Request Checklist

- [ ] **Branch is up to date with the Staging Branch**
- [ ] **The project runs**
- - [ ] You can download and install locally, and run the project locally
- - [ ] All existing and new features run without new bugs
- - [ ] The build script runs without error
- - [ ] (If the project is already deployed to Heroku), the Staging branch can be merged into master branch to be deployed successfully to Heroku and checked for production bugs
- [ ] **Code is consistent**
- - [ ] Linter is used, no error messages
- - [ ] Code is consistent with agreed team style
- - [ ] Naming of files is consistent with project (e.g. all files named with - between words)
- [ ] **Tests are in place**
- - [ ] Test file is in the same folder as the original file, with the extension .test.js
- - [ ] Each new file written has a test file (where possible)
- [ ] **Tests all pass**
- - [ ] All tests should pass locally and on Travis
- - [ ] Edge cases have been considered in tests
- [ ] **Test coverage is maintained**
- - [ ] Project coverage stays > 85%
- - [ ] PR will not bring down coverage by more than 5%
- - [ ] If you are stuck with writing tests, you have assigned @arrested-developer to the PR and added a comment to explain what help is needed
- [ ] **minimal console logs**
- - [ ] Console.log is only used for crucial system messages (e.g. which port server is on).
- - [ ] Any console.logs used for debugging have been removed.
- - [ ] Console.error is used in error handling.
- - [ ] global.console.log and global.console.error are mocked in tests when needed to avoid littering the console

## Merging Pull Requests

- The person that made the pull request is responsible for the final merge, but only after at least one other person from the team has reviewed, assign everyone to review pull requests
