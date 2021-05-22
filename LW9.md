---
# Front matter
lang: ru-RU
title: Текстовый редактор vi
subtitle: ДР по ОС №9
author: Аникин Константин Сергеевич
group: НПИбд-01-20

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

- Получить теоретические и практические навыки работы с текстовым редактором vi

# Задание

- Ознакомиться с теоретическим материалом.

- Ознакомиться с редактором vi.

- Выполнить упражнения, используя команды vi.

# Теоретическое введение 

[[1]](https://docs.altlinux.org/ru-RU/archive/2.3/html-single/junior/alt-docs-extras-linuxnovice/ch02s10.html)

Наилучшим способом уяснить для себя все концепции редактора vi будет запустить его и отредактировать в нем некоторый файл.

vi filename

Редактор vi сейчас находится в командном режиме. Нажмём клавишу i, и редактор перейдёт в режим ввода текста. Вводим текст.

Для выхода из редактора vi без сохранения изменений, сделанных в файле, используется команда :q!. 

Когда вводится команда :, курсор переходит на последнюю строку экрана, и таким образом редактор оказывается в режиме последней строки.

Чтобы сохранить файл, но не выходить из редактора vi, используется команда :w.

Команды для работы с редактором можно найти здесь [[2]](http://rsusu1.rnd.runnet.ru/unix/ucomm/vi.html)

# Выполнение лабораторной работы

## Часть 1

1. Создание папки и файла hello.sh (у меня структура папок организована немного по-другому, чем в описании работы) (рис. 1)

![](https://raw.githubusercontent.com/RituLiot/os-9/main/images/1.png)

*Рис. 1: Создание файла hello.sh*

2. Ввод текста программы, данного в описании работы (рис. 2)

![](https://raw.githubusercontent.com/RituLiot/os-9/main/images/2.png)

*Рис. 2: Заполнение файла hello.sh*

3. Сохранение изменений (рис. 3)

![](https://raw.githubusercontent.com/RituLiot/os-9/main/images/3.png)

*Рис. 3: Сохранение изменений в файле hello.sh*

4. Изменение полномочий файла hello.sh (рис. 4)

![](https://raw.githubusercontent.com/RituLiot/os-9/main/images/4.png)

*Рис. 4: Добавление возможности исполнения файлу hello.sh*

## Часть 2

1. Добавление символа O в текст программы (рис. 5)

![](https://raw.githubusercontent.com/RituLiot/os-9/main/images/6.png)

*Рис. 5: Изменение первого HELL на HELLO*

2. Удаление LOCAL в тексте программы. Сделано в командном режиме через d0 (рис. 6)

![](https://raw.githubusercontent.com/RituLiot/os-9/main/images/8.png)

*Рис. 6: Удаление LOCAL в командном режиме*

3. Ввод local, перемещение к концу файла через G+$, ввод echo $HELLO (рис. 7)

![](https://raw.githubusercontent.com/RituLiot/os-9/main/images/9.png)

*Рис. 7: Добавление local и echo $HELLO*

4. Удаление последней строки в командном режиме, через d0 (рис. 8)

![](https://raw.githubusercontent.com/RituLiot/os-9/main/images/10.png)

*Рис. 8: Удаление последней строки*

5. Отмена последнего действия через u (рис. 9)

![](https://raw.githubusercontent.com/RituLiot/os-9/main/images/11.png)

*Рис. 9: Отмена последнего действия*

6. Сохранение изменений (рис. 10)

![](https://raw.githubusercontent.com/RituLiot/os-9/main/images/12.png)

*Рис. 10: Сохранение изменений*

# Выводы

Материал освоен полностью, работа выполнена без ошибок. Ознакомление с vi прошло успешно.


## Библиографический список:

[1]: [Работа с редактором vi](https://docs.altlinux.org/ru-RU/archive/2.3/html-single/junior/alt-docs-extras-linuxnovice/ch02s10.html)

[2]: [Справочник по редактору vi](http://rsusu1.rnd.runnet.ru/unix/ucomm/vi.html)
