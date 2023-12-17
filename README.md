# Практическая работа №1. 
# Делимся проектом с миром
## Подготовил Исаев М.
## Шпаргалка по работе

---
## Запуск командной строки:
1. *Windows*  - используется программа Git Bash;
2. *Mac OS* - нажать комбинацию клавиш **Cmd+Space**, затем ввести **terminal**;
3. *Linux* - нажать комбинацию клавиш **Ctrl+Alt+T**
---
## Базовые команды в консоли
---
### Навигация
1. ```pwd```  — покажи, в какой я папке;
2. ```ls```  — покажи файлы и папки в текущей папке;
3. ```ls -a``` — покажи также скрытые файлы и папки, названия которых начинаются с символа .;
4. ```cd first-project```  — перейди в папку first-project;
5. ```cd first-project/html``` — перейди в папку html, которая находится в папке first-project;
6. ```cd ..``` — перейди на уровень выше, в родительскую папку;
7. ```cd ~``` — перейди в домашнюю директорию (/Users/Username);
8. ```cd /``` — перейди в корневую директорию.
---
### Работа с файлами и папками

#### Создание
1. ```touch index.html```  — создай файл index.html в текущей папке;
2. ```touch index.html style.css script.js``` — если нужно создать сразу несколько файлов, можно напечатать их имена в одну строку через пробел;
3. ```mkdir second-project```  — создай папку с именем second-project в текущей папке.
#### Копирование и перемещение
1. ```cp file.txt ~/my-dir``` — скопируй файл в другое место;
2. ```mv file.txt ~/my-dir``` — перемести файл или папку в другое место.
#### Чтение
1.```cat file.txt``` — распечатай содержимое текстового файла file.txt.
#### Удаление
2. ```rm about.html``` — удали файл about.html;
3. ```rmdir images```  — удали папку images;
4. ```rm -r second-project``` — удали папку second-project и всё, что она содержит.
---
## Инициализация репрозитория 
1. ```git init``` - Сделать папку репозиторием;
2. ```rm -rf.git``` - Разгитить папку;
3. ```git status``` - Проверка состояние репрозитория.
---
## Добавление файлов в репрозиторий
1. ```git add (пробел) название файла, или пробел . добавить всю папку``` - Подготовка файлов к сохранению
---
## Первый коммит
1. ```git commit -m``` - выполнить коммит;
Сообщение коммита выполняет те же функции — улучшает понимание и упрощает навигацию.<br> Оно пишется после ключа -m в кавычках.
---
## Просмотр истории коммитов
1. ```git log``` - просмотр истории, выводит коммиты в обратном хронологическом порядке — последние коммиты оказываются первыми сверху.
---
##GitHub
---
###Генерация SSH-ключа
1. ```ls -la.sh/``` проверка ключей в домашней директории ~;
2. ```ssh-keygen -t ed25519 -C "электронная почта, к которой привязан ваш аккаунт на GitHub" ``` - генерация ключа SSH  по алгоритму ed25519;
3.```ssh-keygen -t rsa -b 4096 -C "электронная почта, к которой привязан ваш аккаунт на GitHub"``` - генерация ключа SSH по алгоритму 4096.
---
###Связываение локального и удаленного репрозитория
1. ```git remote add origin git@github.com:%ИМЯ_АККАУНТА%/first-project.git```- команда на связывание находится на странице проекта в GitHub;
2. ```git remote -v``` - проверка связи репрозиториев.
---
###Синхронизация репрозиториев
1. ```git push -u origin main``` - или -f
---