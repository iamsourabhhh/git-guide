# GIT

- Backup your current code as zip file.

- To clone the repo on your local
  ```bash
  git clone git@github.com:abhishekmehta1/LXME.git
  ```
- Checkout developer
  ```bash
  git checkout developer
  ```
- To run the project -

  ```bash
  cd LXME
  npm install
  react-native link
  # TO RUN ON ANDROID
  react-native run-android
  # TO RUN ON IOS
  react-native run-ios
  ```

- Remote branches

  - master
  - developer

- Push all the latest stable code on developer branches.

- Don't push on master.

- General Worlflow

  - Make two copies for developer branch on your local, namely developer and your feature branch

  - Make changes on your feature branch

  - To push code on remote developer.

```bash
$ git checkout feature-branch
$ git add .
$ git commit -m "test commit"
# update your local tree
$ git fetch
# rebase with remote developer
$ git rebase origin/developer
# now your feature branch is on top of remote developer
$ git checkout developer
# Update your local developer
$ git pull --rebase
# merge developer with feature branch
git merge feature-branch
```
