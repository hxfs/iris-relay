# Fork Workflow

Branches:

- `upstream` is meant to be regularly updated with the upstream remote https://github.com/linkedin/iris-relay
- `pr` is meant to be used as a PR target (usually the same as upstream)
- `master` includes Wayfair specific things and latest changes.
- `patch` is meant to contain changes which do not include Wayfair specific things (Jenkinsfile, docker-compose.yaml), i.e. it's `master` minus these things.

Pull upstream:

- git remote add upstream git@github.com:linkedin/iris-relay.git
- git checkout upstream
- git pull upstream master

Update ongoing work

- git checkout master
- git merge upstream

Update ongoing patch

- git checkout patch
- git merge master

Prepare PR

- Create an MR from `patch` targeting `pr`
