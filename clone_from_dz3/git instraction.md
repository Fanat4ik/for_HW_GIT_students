
# **<span style="color:#A52A2A"> Инструкция по работе с GIT</span>**
# <image src="logo_Git.jpg" alt="">

Git - это консольная утилита, для отслеживания и ведения истории изменения файлов, в вашем проекте. Чаще всего его используют для кода, но можно и для других файлов. Например, для картинок - полезно для дизайнеров.

С помощью Git-a вы можете откатить свой проект до более старой версии, сравнивать, анализировать или сливать свои изменения в репозиторий.

Репозиторием называют хранилище вашего кода и историю его изменений. Git работает локально и все ваши репозитории хранятся в определенных папках на жестком диске.

## **<span style="color:#8A2BE2"> Настройка git:</span>**
> * ## git config --global user.name "<span style="color:#c5fb03"><ваше имя></span>"
> * ## git config --global user.email "<span style="color:#c5fb03"><адрес_почты@email.com></span>"


## **<span style="color:#8A2BE2"> Команды git:</span>**

## <span style="color:#f97804"> git init</span>

Команда *git init* создаёт git репозиторий в текущей папке

## <span style="color:#f97804"> git add</span>

Команда *git add* добавляет файл в список отслеживаемых (индексируемых) файлов

## <span style="color:#f97804"> git add .</span>

Команда *git add .* (аналогично *git add --all*) добавляет все файлы в список отслеживаемых (индексируемых) файлов


## <span style="color:#f97804"> git commit</span>

Команда *git commit* фиксирует текущую версию файла(ов) 

## <span style="color:#f97804"> git commit -a</span>

Команда *git commit -a* добавляет все файлы в список отслеживаемых (индексируемых) файлов и фиксирует текущую версию файлов

## <span style="color:#f97804"> git commit -m <span style="color:#4682B4"> "комментарий коммита"</span></span>

Команда *git commit -m "комментарий коммита"* фиксирует текущую версию файлов и сразу в этой строке позволяет добавить комментарий

## <span style="color:#f97804"> git status</span>

Команда *git status* показываест состояние репозитория

## <span style="color:#f97804"> git status -s</span>

Команда *git status -s* показываест сокращённый вид состояния файлов в репозитории

## <span style="color:#f97804"> git log</span>

Команда *git log* показывает список commit, дату их создания и автора.

## <span style="color:#f97804"> git log -p</span>

Команда *git log -p* показывает также разницу привнесённую каждым commit

## <span style="color:#f97804"> git show <span style="color:#4682B4"> "хэш коммита"</span></span>

Команда *git show* показывает изменения отдельного commit

## <span style="color:#f97804"> git diff</span>

Команда *git diff* показывает изменения до выполнения инициализации

## <span style="color:#f97804"> git diff --staged</span>

Команда *git diff --staged* показывает разницу между зафиксированным и инициализируемым состоянием

## <span style="color:#f97804"> git diff <span style="color:#4682B4">  <исходная_ветка> <целевая_ветка></span></span>

Команда *git diff <исходная_ветка> <целевая_ветка>* показывает  изменения относительно двух веток.

## <span style="color:#f97804"> git checkout <span style="color:#4682B4"> "хэш коммита"</span></span>

Команда *git checkout* позволяет перемещаться между commit

## <span style="color:#f97804"> git checkout master</span>

Команда *git checkout master* перемещает на вершину ветки мастер

## **<span style="color:#8A2BE2"> Команды для ветвления в GIT:</span>**

## <span style="color:#f97804"> git branch</span>

Команда *<span style="color:#f97804"> git branch</span>* выводит список веток, а также указывает звёздочкой, в какой ветке мы сейчас находимся.

## <span style="color:#f97804"> git branch <span style="color:#4682B4"> "имя ветки"</span></span>

Команда *<span style="color:#f97804"> git branch <span style="color:#4682B4"> "имя ветки"</span></span>* создаёт новую ветку с заданным именем.

## <span style="color:#f97804"> git checkout <span style="color:#4682B4"> "имя ветки"</span></span>

Команда *<span style="color:#f97804"> git checkout <span style="color:#4682B4"> "имя ветки"</span></span>* перемещает на вершину заданной ветки.
Ранее данная команда была описана только для коммитов.

## <span style="color:#f97804"> git checkout -b <span style="color:#4682B4"> "имя ветки"</span></span>

Команда *<span style="color:#f97804"> git checkout -b <span style="color:#4682B4"> "имя ветки"</span></span>* создаёт ветку и сразу  перемещает на вершину созданой ветки

## <span style="color:#f97804"> git merge <span style="color:#4682B4"> "имя ветки"</span></span>

Данная команда *<span style="color:#f97804"> git merge <span style="color:#4682B4"> "имя ветки"</span></span>*, позволяет слить одну ветку в другую, при этом указанная в команде ветка будет слита в ту ветку, в которой сейчас была написана данная команда.

## <span style="color:#f97804"> git branch -d <span style="color:#4682B4"> "имя ветки"</span></span>

Команда *<span style="color:#f97804"> git branch -d <span style="color:#4682B4"> "имя ветки"</span></span>* удаляет указанную ветку, если та была слита с другой.

## <span style="color:#f97804"> git branch -D <span style="color:#4682B4"> "имя ветки"</span></span>

Команда *<span style="color:#f97804"> git branch -D <span style="color:#4682B4"> "имя ветки"</span></span>* удаляет указанную ветку, даже если та не была слита с другой.

## <span style="color:#f97804"> git log --all --oneline</span>

Команда *git log --all --oneline* показывает список commit всех веток в упрощённом виде.

## <span style="color:#f97804"> git log --all --oneline --graph --decorate</span>

Команда *git log --all --oneline --graph --decorate* показывает список commit всех веток в упрощённом виде, а также схематично изоражает струтуру дерева слева от коммитов.

## **<span style="color:#8A2BE2"> Команды для работы с удалённым репозиторием в GIT:</span>**

## <span style="color:#f97804"> git remote</span>

Команда *git remote* позволяет создавать, просматривать и удалять подключения к другим репозиториям.

## <span style="color:#f97804"> git remote -v</span>

Аналогично команде выше, но включает URL-адрес каждого подключения.

## <span style="color:#f97804"> git remote add <span style="color:#4682B4">  <namе(имя)> <url(адрес)> </span> </span>

Создание нового подключения к удаленному репозиторию. После добавления удаленного репозитория имя ＜name＞ можно использовать в качестве удобного ярлыка для адреса ＜url＞ в других командах Git.

## <span style="color:#f97804"> git remote rm <span style="color:#4682B4">  <namе(имя)> </span> </span>

Удаление подключения к удаленному репозиторию с именем ＜name＞.

## <span style="color:#f97804"> git remote rename <span style="color:#4682B4">  <old-namе> <new-namе> </span> </span>

Переименование удаленного подключения с имени ＜old-name＞ на ＜new-name＞.

## <span style="color:#f97804"> git fetch</span>

Команда git fetch загружает коммиты, файлы и ссылки из удаленного репозитория в ваш локальный репозиторий.

## <span style="color:#f97804"> git fetch  <span style="color:#4682B4">  <remotе> </span> </span>

Извлечение всех веток из репозитория. При этом также загружаются все необходимые коммиты и файлы из другого репозитория.

## <span style="color:#f97804"> git fetch  <span style="color:#4682B4">  <remotе> <brаnch> </span> </span>

Аналогично команде выше, но данные извлекаются только для указанной ветки.


## <span style="color:#f97804"> git push  <span style="color:#4682B4">  <remote-namе> <branch-namе> </span> </span>

Этой командой состояние локальной ветки ＜branch-name＞ передается в удаленный репозиторий, обозначенный как ＜remote-name＞.
Чаще видим эту команду в таком виде:

## <span style="color:#f97804"> git push origin master</span>
Отправляем наши изменения в GitHub ветки мастер


## <span style="color:#f97804"> git pull</span>

Команда git pull используется для извлечения и загрузки содержимого из удаленного репозитория и немедленного обновления локального репозитория этим содержимым.

## <span style="color:#f97804"> git pull origin master</span>
Обновляем локальную ветку с сервера
(Подтягиваем изменения из репозитория GitHub)




## <span style="color:#f97804"> git clone <span style="color:#4682B4">  <адрес_удалённого_репозитория> </span> </span>

Клонирует переданный репозиторий на ваш компьютер.
