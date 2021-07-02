# practice-git-2
#Создаем локальный репозиторий tasks-branches ,входим в него и инициируем.
git init
#Создаем файл и добавляем в него текст 
echo "commit_one" >> file.txt
#добавляем данный файл к отслеживанию гитом
git add file.txt
#делаем commit
git commit -m "Commit 1"
#Повторяем процедуру до создания 3 коммита и создаем ветку 
git checkout -b branch1 
#Повторяем процедуру изменения файла и комитим,после чего переключаемся на мастер 
git checkout master
#Также вносим изменения,коммитим, создаем и переключаемся на ветку branch2
git checkout -b branch2 
#Также вносим изменения,коммитим
Проверяем сделанную работу при помощи git log --all --decorate --oneline--graph
#Для удобства создаем алиас 
git config --global alias.g 'log --all --decorate --oneline --graph'

