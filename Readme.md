# Инструкция по работе с Git и удалёнными репозиториями

## Что такое Git?

Git - одна из реализаций распределённых систем контроля версий, имеющая как лольную версионность, так и версионность на сервере. Git является самой популярной системой контроля версий на сегодняшний день.

## Подготовка репозитория
Для того, чтобы создать репозиторий в указанной папке используется команда *git init*. Для этого достаточно написать команду *git init* в папке с будущем репозиторием

## Создание фиксаций
### Просмотр информации о изменениях

Для того, чтобы посмотреть информацию об изменениях, сделанных в текущей ветке, необходимо использовать команду *git status*. Для этого достаточно использовать *git status* в папке с репозиторием

### Добавление файла к коммиту
Для того, чтобы добавить файл к новому коммиту("сохранению") необходимо использовать команду *git add*. Используется она следующим образом: в папке с репозиторием пишем команду *git add <имя файла>*

### Создание коммитов

Для создания новой фиксации необходимо использовать команду *git commit*. Используется она следующим образом: в папке с репозиторием пишется команда *git commit -m "<сообщение к коммиту>"*. Все файлы коммита должны быть предворительно добавлены с помощью команды *git add*. Сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***

## Перемещение между сохранениями
Для перемещения между коммиитами необходимо использовать команду *git checkout*. Используется она следующим образом в папке с репозиторием: *git checkout <номер комиита>*.

## Журнал изменений
Для просмотра журнала изменений необходимо использовать команду *git log*. Для этого нужно в папке с репозиторием написать *git log*

## Ветки в Git
### Создание веток в Git
Для того, чтобы создать новую ветку необходимо использовать команду *git brnach*. Используется она следующим образом в папке с репозиторием: *git branch <название ветки>*.
### Просмотр списка веток
Для того, чтобы просмотреть список веток необходимо использовать команду *git branch*. Для этого в папке с репозиторием надо набрать команду *git branch*

### Переход между ветками
Для того, чтобы перейти на другую ветку необходимо использовать команду *git checkout*. Используется она в папке с репозиторием следующим образом: *git checkout <название ветки>*.

## Слияние веток и разрешение конфликтов
### Слияние веток
Для слияния веток необходимо использовать команду *git merge*. Используется она следующим образом: Для начала ***ОБЯЗАТЕЛЬНО*** перейти на ветку, куда мы сливаем изменения, после чего надо воспользоваться командой *git merge <название сливаемой ветке>*. Слияние может произойти автоматически, а может вознить конфликт. Про разрешение конфликтов смотри дальше.

## Удаление веток
Чтобы удалить ветку необходимо использовать команду "git branch -d <branch_name>"
### Работа с удаленными репозиторями
Существует несколько команд для работы с удаленными репозиториями:  
**git clone** - позволяет склонировать и скачать репозиторий из интернета на ПК пользователя  
**git pull** - позволяет скачать всё из удаленного репозитория и сделать "merge" с текущими данными.
**git push** - позволяет отправить изменения из локального в удаленный репозиторий.

###### The end
