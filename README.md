# Lab Objectives

1. [OWASP Dependency Check](https://github.com/jeremylong/DependencyCheck) scan must be run on each opened pull request
2. Push all successfully checked pull requests to main branch
3. [OWASP Dependency Check](https://github.com/jeremylong/DependencyCheck) scan must be run on each push to main branch
4. Project must use NPM or YARN

# Lab Documentation

[OWASP-prepared action for SCA on GitHub](https://github.com/dependency-check/Dependency-Check_Action) and [automerge-action](https://github.com/marketplace/actions/merge-pull-requests-automerge-action) has been used.

Repository files: 
- [push_main.yml](.github/workflows/push_main.yml) performs scans on each push to main branch
- [pull_open.yml](.github/workflows/pull_open.yml) performs scans on each opened pull request
- [pull_merge.yml](.github/workflows/pull_merge.yml) automerges pull requests to main (triggered by pull_open)

Additionally branch protection has been set to only allow merge when CI has finished.

![Branch protection setup](https://ze.psu.je/137YZN/zrzut-ekranu-2023-12-14-o-11.50.42.png)

Finally auto-merge has been enabled.

![Auto-merge setting](https://ze.psu.je/UYTZr/zrzut-ekranu-2023-12-14-o-13.45.34.png)

NOTE: According to [GitHub documentation](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/incorporating-changes-from-a-pull-request/automatically-merging-a-pull-request#about-auto-merge) only users with r/w permissions to repository are able to auto-merge. Public forks won't merge automagically.

# Todo App

A simple buggy todo app

# Installation
```bash
git clone https://github.com/qxb3/todo-app.git
cd todo-app
npm install #or yarn
```

# Running
```bash
# Running development
npm run dev

# Building
nom run build
```

# Contributing

Just make a pr and hope for the best :)
