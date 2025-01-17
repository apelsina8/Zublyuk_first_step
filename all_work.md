# Инструкция для работы с markdown

## Выделение текста
* Полужирным - обрамляем (**/__)
* Курсивом - обрамляем (*/_)

## Списки
* Для создания ненумерованного списка в начале добавляем (*/-)
* Для нумерованного списка в начале добавляем цыфры (1. 2.)

## Изображения 
Чтобы вставить изображение в текст, достаточно написать следующее: 
![привет это кот](kot.jpg)





# Работа в Git и базовые команды к нему.

## Что такое Git и с чем его едят?

Git - одна из популярных программ для работы с системой контроля версий. Облегчает паралельное производство продукта в большом коллективе. Имеет возможность создавать как локальные, так и удалённые репозитории.

## Создание репозитория
Для возможности работы с *Git* необходимо создать репозиторий, путём ввода команды - *git init*. Тем самым в выбранной папке создадуться скрытые файлы являющиеся непосредственно репозиторием.

## Включение данных в репозиторий и их сохранение
* Для добарления файлов в репозиторий применяется команда - *git add "имя файла"*, фиксируя текущий файл как рабочий и запоминая его состояние.
* Следующая основная команда - *git commit *, фиксирующая текущее состояние файла в системе и записывающая его индивидуальный *id*.

## Дополнительные вспомогательные программы
1. *git status* - показывает изменения позошедшие с последнего сохранения и какие элементы ещё не сохранены.
2. *git log* - вызывает список всех commit-ов, произведённых с репозиторием, указывая кто сохронял, когда и *id* каждого сохранения.
3. *git diff* - показывает разницу изменения между 2 выбранными commit-ами. Если в конце команды вписано одно *id*, то покажет между ним и текущим, если 2, то выдаст разницу именений между ними.

4. *git checkout* **id** - вызывает выбранный commit, с которым можно проводить любые манипуляции. Для возврата к последнему вместо *id* вписывается *masster*.

## Команды для работы с ветками 
1. *git branch* - команда для прсмотра имеющихся веток, если в конце добавить имя, то создаёт новую ветку с данным именем.
2. *git checkout "name"* - переход на выбранную ветку. Если добавить перед _"name"_ конструкцию (*-b*), то сразу создасться новая ветка (если таковой не вуществовало) и произойдёт переход на неё.
3. *git branch -d "name"* - команда служит для удаления выбранной ветки. Вместо *(-d)* можно использовать конструкцию (-D), которая производит принудительное удаление ветки, в независимости от условий (*пример* ветка не добавлена в остальную, или слияние с не разрешённым конфликтом)
4. *git log --graph* - команда вызывает список commit-ов с отображением ветвления и слияния веток.
5. *git merger "name"* - сливает выбранную ветку в ТЕКУЩУЮ. При возникновении конфлика предлагает выбрать в ручную один из вариантов, или оставить оба.


Тест для ознакомления

Тест №2 проверка на принятие удалённым репоз.

Тест №3 снова проверка push
