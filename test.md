# Инструкция по работе с GIT

Git - это консольная утилита, для отслеживания и ведения истории изменения файлов, в вашем проекте. Чаще всего его используют для кода, но можно и для других файлов. Например, для картинок - полезно для дизайнеров.

С помощью Git-a вы можете откатить свой проект до более старой версии, сравнивать, анализировать или сливать свои изменения в репозиторий.

Репозиторием называют хранилище вашего кода и историю его изменений. Git работает локально и все ваши репозитории хранятся в определенных папках на жестком диске.

## **<span style="color:blue"> Настройка git:</span>**
> * ## git config --global user.name "<span style="color:#c5fb03"> <ваше имя></span>"
> * ## git config --global user.email "<span style="color:#c5fb03"> <адрес_почты@email.com></span>"


## **<span style="color:blue"> Команды git:</span>**

## <span style="color:#f97804"> git init</span>

Команда *git init* создаёт git репозиторий в текущей папке

## <span style="color:#f97804"> git add</span>

Команда *git add* добавляет файл в список отслеживаемых (индексируемых) файлов

## <span style="color:#f97804"> git add .</span>

Команда *git add .* добавляет все файлы в список отслеживаемых (индексируемых) файлов


## <span style="color:#f97804"> git commit</span>

Команда *git commit* фиксирует текущую версию файла(ов) 

## <span style="color:#f97804"> git commit -a</span>

Команда *git commit -a* добавляет все файлы в список отслеживаемых (индексируемых) файлов и фиксирует текущую версию файлов

## <span style="color:#f97804"> git status</span>

Команда *git status* показываест состояние репозитория

## <span style="color:#f97804"> git status -s</span>

Команда *git status -s* показываест сокращённый вид состояния файлов в репозитории

## <span style="color:#f97804"> git log</span>

Команда *git log* показывает список commit, дату их создания и автора.

## <span style="color:#f97804"> git log -p</span>

Команда *git log -p* показывает также разницу привнесённую каждым commit

## <span style="color:#f97804"> git show</span>

Команда *git show* показывает изменения отдельного commit

## <span style="color:#f97804"> git diff</span>

Команда *git diff* показывает изменения до выполнения инициализации

## <span style="color:#f97804"> git diff --staged</span>

Команда *git diff --staged* показывает разницу между зафиксированным и инициализируемым состоянием

## <span style="color:#f97804"> git checkout</span>

Команда *git checkout* позволяет перемещаться между commit

## <span style="color:#f97804"> git checkout master</span>

Команда *git checkout master* возвращает на последнюю версию commit