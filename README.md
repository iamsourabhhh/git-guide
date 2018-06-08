# GIT

- Backup your current code as zip file.

- To clone the repo on your local
  ```bash
  git clone git@github.com:abhishekmehta1/LXME.git
  ```
- Checkout develop
  ```bash
  git checkout develop
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
  - develop

- Push all the latest stable code on develop branches.

- Don't push on master.

- General Worlflow

  - Make two copies for develop branch on your local, namely develop and your feature branch

  - Make changes on your feature branch

  - To push code on remote develop.

```bash
$ git checkout feature-branch
$ git add .
$ git commit -m "test commit"
# update your local tree
$ git fetch
# rebase with remote develop
$ git rebase origin/develop
# now your feature branch is on top of remote develop
$ git checkout develop
# Update your local develop
$ git pull --rebase
# merge develop with feature branch
git merge feature-branch
```
