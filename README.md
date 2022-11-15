# Выявление болезни по звуку дыхания легких


# Как работаем:
- клонируем репозиторий, можно сразу вдобавок форкнуть, чтобы отслеживать было проще
~~~
git clone git@github.com:Totenkaf/disiase_breathing_identification.git
~~~
- создаем локально ветку со своим именем и приставкой dev:
~~~
git checkout -b Artem-dev
~~~
- называем коммиты адекватно:
~~~
git commit -m 'make setup file'
~~~
- если вдруг написали с ошибкой или не так, а коммит вы уже сделали, можно переименовать:
~~~
git commit --amend -m 'new'
~~~
- после добавления коммита, нужно создать подключение к удаленной ветке:
~~~
git push --set-upstream origin Artem-dev
~~~
- давайте вести разработку в своих ветках, сливать все в отдельных, если все работает - заливать в main  

- заливать в мейн - делайте ребейз, в дальнейшем при работе в своей ветке, тоже делайте ребейз, избежим конфликтов
~~~
git checkout main, git pull, git checkout <your branch name>
git rebase -i main
~~~

- Скачать, разархивировать и удалить архив с данными:
~~~
sudo apt-get install wget -y
wget https://ml_project.hb.bizmrg.com/nn_project/breath_diseases.zip -P data/ 
unzip data/breath_diseases.zip && rm -rf data/breath_diseases.zip
~~~