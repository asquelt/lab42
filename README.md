# Lab Objectives

1. [OWASP Dependency Check](https://github.com/jeremylong/DependencyCheck) scan must be run on each opened pull request
2. Push all successfully checked pull requests to main branch
3. [OWASP Dependency Check](https://github.com/jeremylong/DependencyCheck) scan must be run on each push to main branch
4. Project must use NPM or YARN

# Lab Documentation

[OWASP-prepared action for SCA on GitHub](https://github.com/dependency-check/Dependency-Check_Action) and [automerge-action](https://github.com/marketplace/actions/merge-pull-requests-automerge-action) has been used.

Repository file (.github/workflows/push_main.yml) performs scans on each push to main branch.

Repository file (.github/workflows/pull_open.yml) performs scans on each opened pull request.

Repository file (.github/workflows/pull_merge.yml) accepts the merge.

Additionally branch protection has been set to only allow merge when CI has finished.

![Branch protection setup](https://ze.psu.je/137YZN/zrzut-ekranu-2023-12-14-o-11.50.42.png)

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

Just make a pr :)

```
     ...           ...           ...           ...
    (o o)         (- o)         (o -)         (- -)
ooO--(_)--Ooo-ooO--(_)--Ooo-ooO--(_)--Ooo-ooO--(_)--Ooo-

     ...           ...           ...           ...
    (* *)         (x x)         (o O)         (O o)
ooO--(_)--Ooo-ooO--(_)--Ooo-ooO--(_)--Ooo-ooO--(_)--Ooo-

     ...           ___           ,,,           ooo
    ( oo)         (o o)         (o o)         (o o)
ooO--(_)--Ooo-ooO--(_)--Ooo-ooO--(_)--Ooo-ooO--(_)--Ooo-

     ===           +++           ###          -*~*-
    (o o)         (o o)         (o o)         (o o)
ooO--(_)--Ooo-ooO--(_)--Ooo-ooO--(_)--Ooo-ooO--(_)--Ooo-

     ***           |||          -`^'-          /777
    (o o)         (o o)         (o o)         (o o)
ooO--(_)--Ooo-ooO--(_)--Ooo-ooO--(_)--Ooo-ooO--(_)--Ooo-

     _/7           )))           (((           xxx
    (o o)         (o o)         (o o)         (o o)
ooO--(_)--Ooo-ooO--(_)--Ooo-ooO--(_)--Ooo-ooO--(_)--Ooo-
                                  _
  `  ___  '        @__           ((_           >X<
 -  (O o)  -      (o o)         (o o)         (o o)
ooO--(_)--Ooo-ooO--(_)--Ooo-ooO--(_)--Ooo-ooO--(_)--Ooo-

     '*`          \-^-/          ^^^           )|(
    (o o)         (o o)         (o o)         (o o)
ooO--(_)--Ooo-ooO--(_)--Ooo-ooO--(_)--Ooo-ooO--(_)--Ooo-

                                 (           |
     \|/           &&&           _)_         |.===.
    (o o)         (o o)         (o o)        {}o o{}
ooO--(_)--Ooo-ooO--(_)--Ooo-ooO--(_)--Ooo-ooO--(_)--Ooo-

    ( ( (                           ...           |"|
  '. ___ .'       ,,,,,        o,*,(o o)         _|_|_
 '  (> <) '      /(o o)\      8(o o)(_)Ooo       (o o)
ooO--(_)--Ooo-ooO--(_)--Ooo-ooO-(_)---Ooo----ooO--(_)--Ooo-

      _                          ___         .      .
    _|_|_        __MMM__        .|||.      .  .:::.
    (o o)         (o o)         (o o)        :(o o):  .
ooO--(_)--Ooo-ooO--(_)--Ooo-ooO--(_)--Ooo-ooO--(_)--Ooo-

                   ___         _     _          ___
     vvv          /\#/\      o' \,=./ `o       /_\ `*
    (0~0)        /(o o)\        (o o)         (o o)
ooO--(_)--Ooo-ooO--(_)--Ooo-ooO--(_)--Ooo-ooO--(_)--Ooo-

    _   _      #   ___      #                 #     ___
   '\\-//`     #  <_*_>     #=ooO=========Ooo=#    '/_\
    (o o)      #  (o o)     #  \\  (o o)  //  #    (o o)
ooO--(_)--Ooo--8---(_)--Ooo---------(_)--------ooO--(_)--Ooo-

     !!!                                        o
  `  _ _  '     `  _ ,  '       ()_()        ` /_\ '
 -  (OXO)  -   -  (o)o)  -      (o o)       - (o o) -
ooO--(_)--Ooo--ooO'(_)--Ooo-ooO--`o'--Ooo-ooO--(_)--Ooo-

     ___       #  #  #  #       _   _             .
   .'_#_`.     #  #..#  #      (_)-(_)        ,-_-|
   |[o o]|     #  #O #) #       (o o)        ([o o])
ooO--(_)--Ooo-o#O-#(_#--#oo-ooO--(_)--Ooo-ooO--(_)--Ooo-

                     n
    ((__))      ____/_\____
     (00)          (z z)
nn--(o__o)--nn-ooO--(_)--Ooo-

```
