---
## Front matter
title: "Командная оболочка Midnight Commander"
author: "Ыбырай Роза"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Освоение основных возможностей командной оболочки Midnight Commander. Приобретение навыков практической работы по просмотру каталогов и файлов; манипуляций
с ними.

# Задание

Изучить возможности midnight commander.

# Выполнение лабораторной работы
## Задание по mc

1. Изучение информаций о mc, вызвав в командной строке man mc

![Рис.1: man mc](image/lab7.1.jpg){ #fig:001 width=70% }

2. Запущение из командной строки mc, изучение его структуру и меню.

![Рис.2: страница mc](image/lab7.2.jpg){ #fig:002 width=70% }

3. Выполнение нескольких операций в mc, используя управляющие клавиши (операции с панелями; выделение/отмена выделения файлов, копирование/перемещение файлов, получение информации о размере и правах доступа на файлы и/или каталоги и т.п.)

![Рис.3: выделение](image/lab7.3.jpg){ #fig:003 width=70% }

![Рис.4: отмена выделения](image/lab7.4.jpg){ #fig:004 width=70% }

![Рис.5: копирование](image/lab7.5.jpg){ #fig:005 width=70% }

![Рис.6: перемещение](image/lab7.6.jpg){ #fig:006 width=70% }

![Рис.7: удаление](image/lab7.7.jpg){ #fig:007 width=70% }

![Рис.8: поиск файлов](image/lab7.8.jpg){ #fig:008 width=70% }

![Рис.9: просмотр](image/lab7.9.jpg){ #fig:009 width=70% }

4. Выполнение основных команд меню левой и правой панели

![Рис.10: Быстрый просмотр](image/lab7.10.jpg){ #fig:010 width=70% }

![Рис.11: информация](image/lab7.11.jpg){ #fig:011 width=70% }

![Рис.12: дерево каталогов](image/lab7.12.jpg){ #fig:012 width=70% }

![Рис.13: формат списка файлов](image/lab7.13.jpg){ #fig:013 width=70% }

![Рис.14: фильтр](image/lab7.14.jpg){ #fig:014 width=70% }

5. Используя возможности подменю Файл , выполните:
	-  просмотр содержимого текстового файла;
	-  создание каталога;
	-  копирование в файлов в созданный каталог.

![Рис.15: просмотр содержимого текстового файла](image/lab7.15.jpg){ #fig:015 width=70% }
![Рис.16: создание каталога](image/lab7.16.jpg){ #fig:016 width=70% }
![Рис.17: копирование в файлов в созданный каталог](image/lab7.17.jpg){ #fig:015 width=70% }

6. С помощью соответствующих средств подменю Команда осуществите:
	- поиск в файловой системе файла с заданными условиями (например, файла содержащего строку main);
	- выбор и повторение одной из предыдущих команд;
	- переход в домашний каталог;
	- анализ файла меню и файла расширений

![Рис.18: файлы содержащие строку main](image/lab7.18.jpg){ #fig:015 width=70% }
![Рис.19: история](image/lab7.19.jpg){ #fig:019 width=70% }
![Рис.20: файл расширений](image/lab7.20.jpg){ #fig:020 width=70% }
![Рис.21: файл меню](image/lab7.21.jpg){ #fig:021 width=70% }

7. Вызовить подменю Настройки . Освоить операции, определяющие структуру экрана mc
(Full screen, Double Width, Show Hidden Files и т.д.)

![Рис.22: show hidden files](image/lab7.22.jpg){ #fig:022 width=70% }
![Рис.23: full screen](image/lab7.23.jpg){ #fig:023 width=70% }

## Задание по встроенному редактору mc
1. Создать текстовой файл text.txt

![Рис.24: создание файла text.txt](image/lab7.24.jpg){ #fig:024 width=70% }

2. Открыть этот файл с помощью встроенного в mc редактора.

![Рис.25: открыть файл с mc](image/lab7.25.jpg){ #fig:025 width=70% }

# Выводы

В данной работе мы приобрели практические навыки по просмотру каталогов и файлов, манипуляций с ними.
:::
