# _Инструкция по работе с **Git**_

## Предварительная настройка Git
Чтобы "представиться программе Git нужно ввести команды:

    git config --global user.name "name"
    git config --global user.email "email"
## Создание репозитория 
Чтобы инициализировать новый репозиторий, нужно ввести команду 

    git init 
## Добавление в индекс
Чтобы добавть измнения в индекс (для фиксации в следующем коммите) нужно ввести команду:

    git add "file name"

## Фиксация изменений
Чтобы зафиксировать измненения, добавленные в индекс, нужно ввести команду:

    git commit 
Чтобы оставить сообщение при фиксации, нужно в команде поставить флажок -m:

    git commit -m "текст сообщения"

Чтобы пропустить этап индексирования изменений в файле, нужно в команде поствить фложок -а:

    git commit -a

Чтобы объединить обе команды, нужно в команду поставить оба флажка -am:

    git commit -am "текст сообщения" 
## Проверка статуса
Чтобы узнать, какие файлы изменились, но не индексировались, нужно ввести команду:

    git status
## Проверка журнала изменений
Чтобы посмотреть историю измненения проекта с подписями, нужно ввести команду:

    git log

Чтобы посмотреть журнал измненения проекта без подписей в одну строчку, нужно ввести команду:

    git log --oneline 

Чтобы посмотреть журнал изменений проекта на всех ветках с подписью автора коммита, нужно ввести команду:

    git log --all


Чтобы посмотреть журнал изменений проекта на всех ветках без подписи автора, нужно ввести команду:

    git log --all --oneline

 ## Определение разницы между коммитами

Для просмотра различий между разными версиями используется команда:

    git diff <hash1> <hash2>

Если ввести команду без параметров:

    git diff

будет показана разница между текущим состоянием репозитория и последним закоммиченным.

## Перемещение между коммитами

Чтобы переместиться на конкретный коммит, нужно ввести команду:

    git checkout hash

hash - идентификатор коммита, достаточно ввести от 4 до 8 знаков.

Чтобы переместиться на последнюю версию репозитория, нужно ввести команду:

    git checkout master
    