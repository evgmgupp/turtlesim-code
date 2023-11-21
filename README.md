
### Подписка на ростопик

turtlesubscribe.py - цель этого скрипта - прочитать положение (Pose) черепахи. Нам нужно будет подписаться на /turtle1/Pose тему.

### Перемещение черепахи
move_turtle.py - Цель здесь - заставить черепаху двигаться с линейной скоростью(м/с) и угловой скоростью (рад/с). Нам нужно передать эти два значения в качестве аргументов в терминале.

### Линейное перемещение черепахи
turtlemove.py - Цель здесь - переместить черепаху с помощью ростопика cmd_vel. Нам нужно будет опубликовать ростопик.

### Множество целей
turtlepath.py - Переход к 5 различным точкам. 

### Описание действий
1.	Добавим SSH-ключ на Github. Создаем ключи в терминале командой: _ssh-keygen_. Копируем публичный ключ на Github (Settings – SSH and GPG keys – New SSH key).
2.	Создадим токен доступа через https: Перейдем в Settings – Developer settings – Fine-grained token – new token
3.	Создадим папку командой: _mkdir turtlesim-code_
4.	Перейдем в паку _cd turtlesim-code_
5.	Создадим файл командой: _touch README.md_ и две папки _mkdir scripts1_, _mkdir scripts2_
6.	В папке _scripts1_ создадим файл _touch turtlesubscribe.py_  и  в редакторе напишем код, также создадим файл _README.md_.
7.	В папке _scripts2_ создадим файлы: _move_turtle.py_, _turtlemove.py_, _turtlepath.py_ и в редакторе напишем код, также создадим _README.md_.
8.	Напишем описание файлов в _README.md_.
9.	Работа c Git. Указываем имя и адрес электронной почты _git config --global user.name “Evgenii”_ и _git config --global user.email evgmgupp@gmail.com_
10.	Создание репозитория в существующем каталоге. Переходим в каталог _turtlesim-code_ и вводим команду: _git init_. Если ввести команду _git status_ то должны появиться Неотслеживаемые файлы: _README.md_, _scripts1/_, _scripts2/_.
11.	Добавим в отслеживаемые файлы: _git add README.md_ и папку _git add scripts1_
12.	Зафиксируем свои изменения: _git commit -m “Add README.md and scripts1”_
13.	На Github создадим репозиторий _turtlesim-code_. И настроим локальный репозиторий с удаленным введя команду: _git remote add origin https://github.com/evgmgupp/turtlesim-code.git_ далее команду:  _git remote show origin_. Так как настроили ранее ssh, то пароль не требуется.
14.	Отправим проект в удаленный репозиторий командой: _git push -u origin master_
15.	Создадим отдельную ветку. Команда: _git branch scripts2_. Если введем команду _git branch_, то увидим ветку _master_ и _scripts2_. Перейдем на ветку scripts2: _git checkout scripts2_
16.	Добавим папку в ветку: _git add scripts2_ и _git commit -m "Add scripts2"_
17.	Перенесем ветку в удаленный репозиторий _git push_ (При создании новой ветки: _git push --set-upstream origin scripts2_)
18.	Перейдем на основную ветку: _git checkout master_
19.	Добавим ветку _scripts2_ в master ветку: _git merge scripts2_ 
20.	Отправим проект в удаленный репозиторий командой: _git push_
21.	В файл _README.md_ добавим описание действий: _nano README.md_
22.	Примем изменения: _git commit -am “New description README.md”_ 
23.	Отправим проект в удаленный репозиторий командой: _git push_
