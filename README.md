# GIT OVERVIEW
 
- `git init` : inicjuje repo git w danym katalogu
- `git status` : wyświetla informacje o repo
- `git add <FILE>` : adds <FILE> to the staging area
- `git commit` : zapisuje "staging area" jako commit
     - `git commit -m "MESSAGE"`: Dodaje commit z waidomościa <MESSAGE>
- `git log` : Pokazuje historię logów
    - `git log -oneline` : Zwięzła wersja
- `git diff` : Pokazuje różnice w plikach między obecną wersją, a poprzednnią w repo
    - `git diff --staged` : Pokazuje różnice między plikami w staged area
- `git diff HEAD~<N>` : Porownuje do commitu <N> temu
- `git diff <SHA> <FILE>` : Porownuje do pliku <FILE> z commitu o numerze <SHA>
- `git checkout <SHA> <FILE>` : Wraca do pliku <FILE> z commitu <SHA>
- `git checkout <SHA>`' : Wraca do commitu <SHA>
- `git checkout main` : Powrót do ooryginalnego początku

- `.gitignore` : Plik z listą regexpow plików, których nie umieszcza się w commicie
- `.gitkeep` : Konwencja - by dodać katalogi (katalogi puste nie sa dodawane)

## REMOTES:

- `git remote add <NAME> <URL>` : <NAME> zwykle to "origin", URL - to repo do githuba
- `git push <WHERE> <WHAT>` : local repo -> remote
- `git pull <WHERE> <WHAT>` : remote repo -> local

## BRANCHES:
 
How to fix master -> main
 1. `git checkout -b main`
 2. `git push origin main`
 3. Fix default branch in Github
 
 
# 2021-05-25 GIT Basics

- `git init`: initialize git repo in current location
- `git status`: gives you the status
- `git add <FILE>`: adds <FILE> to the staging area
- `git commit`: commits files from staging area
    - `git commit -m "MESSAGE"`: commit without opening editor
- `git log`: show you commit history
    - `git log --oneline`: condensed history

- `git diff`: gives you the difference
    - `git diff --staged`: diff files in the staging area

- `git diff HEAD~2`: diff 2 commits ago
- `git diff <SHA> <FILE>`: diff a file against a specific commit

- `git checkout <SHA> <FILE>`: revert <FILE> from <SHA> to current time
- `git checkout <SHA>` move you to <SHA>
    - `git checkout main`: go back to main starting point

- `.gitignore`: file that pattern matches files to ignore
- `.gitkeep`: convention to keep a empty folder

## Remotes

- `git remote add <NAME> <URL>`: <NAME=origin> point to the remote <URL>
- `git push <WHERE> <WHAT>`: local repo -> remote
- `git pull <WHERE> <WHAT>`: remote -> local

## BRANCHES

How to fix master -> main

1. `git checkout -b main`
2. `git push origin main`
3. fix default branch in github
