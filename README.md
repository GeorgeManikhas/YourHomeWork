# Добрый день, уважаемые студенты! 
  При выполнении данной работы от вас требуется дополнить мой репозиторий, добавив в него свой файл с инструкцией по работе с git. Помните, что добавление файла - такой же процесс изменения репозитория, как и изменения внутри конкретных файлов и не пугайтесь этого :)

  P.S. Называйте добавляемые файлы своими фамилиями(только на английской раскладке), чтобы мне было проще их идентифицировать. И не забудьте сделать скрин окна с pullrequest, на сайт GB необходимо отослать именно этот скрин, чтобы работа была окончательно завершена.

  P.P.S. Не забывайте, что отправляем на pullrequest мы побочные ветки!




# George Manikhas changes

# Конспект по работе с GIT
## Git является утилитой контроля версий и нужен для ведения истории изменения файла, дополнительно, Git позволяет отслеживать все сохраненные версии файла и иметь доступ к каждой из них.
* Для работы с Git используются консольные команды, некоторые из которых мы рассмотрим ниже:
* git --version - используется для проверки текущей версии git, так же с этой командой проще всего понять правильно ли установлен и работает ли git.
* git init - команда инициализирующая работу программы внутри папки, в которой инициализирован git.
* git add (название файла) - начинает отслеживать выбранный файл.
* git commit -m "" - команда, фиксирующая изменения в файле. "-m" является комментарием к команде, а внутри ковычек пишется название коммита.
* git status - проверка статуса файла.
* git log - вызов журнала изменений.
* git checkout - позволяет обращаться к любой из сохраненных версий файла, адрес котрого можно найти в git log.

## Для сохранения файла в git нужно использовать определенную последовательность действий:
 1. изменить файл
 2. сохранить файла на компьютере (cntrl+s)
 3. использовать команду git add
 4. использовать команду git commit

## Для перемещения между версиями файла нужно использовать следующую последовательность дейтсвий:
1. вызвать журнал изменений (git log)
 2. выбрать нужную версию файла по названию коммита и скопировать ее номер целиком либо первые 4 симовла 
 3. использовать команду git checkout и вставить номер коммита
* Для возвращения к актуальной версии файла нужно использовать команду git checkout master.



# Lesson 2



### Создание веток

Для создания новой ветки используется команда __git branch *branch_name*__. 

Для ознакомления с существующими ветками в репозитории используется команда __git branch__. 

Для удаления веток используется команда __git branch -d *название ветки*__.

Для перемещения между ветками следует использовать команду __git checkout *название ветки*__. В основную (главную) ветку можно вернуться вписав в пункт название слово __master__.

Ветвеление удобно использовать для делигирования работы и разделения ее между участниками проекта. С помощью веток просто и удобно собирать проект, как пазл, воедино. 

### Слияние веток 

Для объединения веток требуется использовать команду __git merge *имя ветки*__. __!!!  Необходимо находиться на ветке master  !!!__

Слияние веток происходит посредством добавления к основной ветке __master__ добавочных (второстепенных)
веток, название которых может быть любым и устанавливается разработчиком. команду см. выше. 
Важно добавить, что при слиянии необходимо находиться на главной ветке __master__. 

### Возникновение и решение конфликтов

Если изменения в отдельных ветках затрагивают общую часть документа, то это приводит к конфликту при слиянии. Конфликт возникает, если на обеих ветвях был произведен __commit__ и для решения таких конфликтов нужно вмешательство разработчика.
Решаются конфликты очень просто, нужно определиться, какая версия файла подходит больше, либо же оставь обе версии. 
