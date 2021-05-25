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
 
 
