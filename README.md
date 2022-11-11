# Выявление болезни по звуку дыхания легких


# Как работаем:
- клонируем репозиторий git clone git@github.com:Totenkaf/disiase_breathing_identification.git
- создаем локально ветку со своим именем и приставкой dev git checkout -b Artem-dev
- называем коммиты адекватно: git commit -m 'make setup file'
- если вдруг написали с ошибкой или не так, а коммит вы уже сделали, можно переименовать: git commit --amend -m 'new'
- после добавления коммита, нужно создать подключение к удаленной ветке: git push --set-upstream origin Artem-dev
- давайте вести разработку в своих ветках, сливать все в отдельных, если все работает - заливать в main  

- заливать в мейн - делайте ребейз
- git checkout main, git pull, git checkout <your branch name>
- git rebase -i main