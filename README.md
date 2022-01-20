http://webdesign.ru.net/article/pravila-oformleniya-fayla-readmemd-na-github.

1) Посмотреть где я: `pwd`

2) Создать папку: `mkdir foldername`

3) Зайти в папку: `cd foldername`

4) Создать 3 папки: `mkdir foldername_1 foldername_2 foldername_3`

5) Зайти в любоую папку: `cd foldername_1`

6) Создать 5 файлов (3 txt, 2 json): `touch/> file_1.txt file_2.txt file_3.txt file_1.json file_2.json`

7) Создать 3 папки: `mkdir foldername_4 foldername_5 foldername_6`

8) Вывести список содержимого папки: `ls`

+ Открыть любой txt файл: `vim file_1.txt`

+ написать туда что-нибудь, любой текст: `i` , вносим изменения

+ сохранить и выйти: `ESC-->:wq`

9) Выйти из папки на уровень выше: `cd ..`

10) Переместить любые 2 файла, которые вы создали, в любую другую папку: `mv filename_1 filename_2 foldername(куда перемещаем в рамках текущей директории)/адрес папки назначения`

11) Скопировать любые 2 файла, которые вы создали, в любую другую папку: `cp filename_1 filename_2 foldername(куда копируем в рамках текущей директории)/адрес папки назначения`

12) Найти файл по имени: `find filename`

13) Просмотреть содержимое в реальном времени (команда grep): `поиск текста в файле по содержимому (https://routerus.com/how-to-use-grep-command-to-search-files-in-linux/)`

14) Вывести несколько первых строк из текстового файла: `head -необходимое число строк filename (например head -3 f_4.txt   выведет первые 3 строки из файла  f_4.txt)`

15) Вывести несколько последних строк из текстового файла: `tail -необходимое число строк filename (например tail -3 f_4.txt   выведет последние 3 строки из файла  f_4.txt)`

16) Просмотреть содержимое длинного файла (команда less) изучите как она работает: `less позволяет перематывать текст не только вперёд, но и назад, осуществлять поиск в обоих направлениях, переходить сразу в конец или в начало файла.Особенность less заключается в том, что команда не считывает текст полностью, а загружает его небольшими фрагментами.`

17) Вывести дату и время: `date`

=========

Задание *
1) Отправить http запрос на сервер. 
http://162.55.220.72:5005/object_info_3?name=Vadim&age=32&salary=1000 : curl 'http://162.55.220.72:5005/object_info_3?name=Vadim&age=32&salary=1000'

2) Написать скрипт который выполнит автоматически пункты 3, 4, 5, 6, 7, 8, 13

-создаем текстовый файл skript.txt, открываем его черз опертор vim, пишем скрипт:

`#!/bin/bash
# комментарий
cd directory
mkdir foldername_1 foldername_2 foldername_3
cd foldername_1
touch file_1.txt file_2.txt file_3.txt file_5.json file_6.json
mkdir foldername_4 foldername_5 foldername_6
mv file_1.txt file_5.json foldername_6`

-делаем файл исполняемым: `chmod ugo+x skript.txt`

-запускаем скрипт: `./skript.txt`

Проверил, работает)

    СТРУКТУРА БАГРЕПОРТА
1) TITLE/SUMMARY-котрокое описание проблемы, явно указывающее на причину и тип ошибочной ситуации.
2) PROJECT-название тестируемого проекта.
3) COMPONENT-название части или функции тетструемого продукта.
4) VERSION-версия продукта на которо найдена ошибка.
5) SEVERITY(СЕРЬЕЗНОСТЬ):
	S1 блокирующий (blocker)
	S2 Критический (Critical)
	S3 Значительный (Major)
	S4 Незначительный (Minor)
	S5 Тривиальный (Trivial)
6) PRYORITY(ПРИОРИТЕТ):
	P1 Высокий (hight)
	P2 Средний (Medium)
	P3 Низкий (low)
7) STATUS(СТАТУС)-зависит от используемой процедуры и жизненного цикла.
8) AUTHOR-создатель баг-репорта.
9) ASSIGNET TO-сотрудник, назначенный на решение проблемы.
10) ОКРУЖЕНИЕ-операционная сиситема, сервиспак, для web-приложений-имя и версия браузера, и т.д.
11) STEPS-шаги, по которым можно легко воспроизвести ситуацию.
12) ФАКТИЧЕСКИЙ РЕЗУЛЬТАТ-результат полученный после воспроизведения шагов.
13) ОЖИДАЕМЫЙ РЕЗУЛЬТАТ-ожидаемый правильный результат.
14) ATTACHMENT-файл с логами, скриншот, любой другой документ который поможет установить причину ошибки или указать на способ решения проблемы.

