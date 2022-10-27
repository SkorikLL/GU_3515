# Описание нашего проекта
## GU_3515

# Инструкция для работы с Git и удалёнными репозиториями
## Что такое Git?
*Git* - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.
## Подготовка репозитория
Для создание репозитория необходимо выполнить команду *git init*  в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)
## Создание коммитов
### Git add
Для добавления измений в коммит используется команда *git add*. Чтобы использовать команду *git add* напишите *git add <имя файла>*
### Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда *git status*. Для этого необходимо в папке с репозиторием написать *git status*, и Вы увидите были ли измения в файлах, или их не было.
### Создание коммитов
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так: *git commit -m "<сообщение к коммиту>*. Все файлы для коммита должны быть ***ДОБАВЛЕНЫ*** и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.
## Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с пепозиторием следующим образом: *git checkout <номер коммита>*
## Журнал изменений
Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием
## Ветки в Git

Для того, чтобы создать ветку, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*

Для того чтобы дабавить ветку в текущую ветку используется команда *git merge <name branch>*

Для удаления ветки ввести команду "git branch -d 'name branch'"

## Объединение веток
Слияние используется в Git, чтобы собрать воедино разветвленную историю. Команда git merge выполняет слияние отдельных направлений разработки, созданных с помощью команды git branch, в единую ветку.

Обратите внимание: все приведенные ниже команды выполняют слияние в текущую ветку, в то время как целевая ветка остается без изменений. Поэтому команда git merge часто используется в сочетании с командами git checkout (для выбора текущей ветки) и git branch -d (для удаления устаревшей целевой ветки).

## Отмена изменений (git reset)
Команда git reset — это сложный универсальный инструмент для отмены изменений. Она имеет три основные формы вызова, соответствующие аргументам командной строки --soft, --mixed, --hard. Каждый из этих трех аргументов соответствует трем внутренним механизмам управления состоянием Git: дереву коммитов (HEAD), разделу проиндексированных файлов и рабочему каталогу.