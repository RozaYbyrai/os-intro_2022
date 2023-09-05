---
## Front matter
title: "Поиск файлов. Перенаправление ввода-вывода. Просмотр запущенных процессов"
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

Ознакомление с инструментами поиска файлов и фильтрации текстовых данных.
Приобретение практических навыков: по управлению процессами (и заданиями), по
проверке использования диска и обслуживанию файловых систем.

# Задание

1. Изучить перенаправление ввода вывода.
2. Изучить работу фильтров и команду поиска.
3. Ознакомиться с управлением процессами и их получение.
4. Ознакомиться с командами df du.

# Выполнение лабораторной работы

## 1. Осуществили вход в систему, используя соответствующее имя пользователя. Записали в файл file.txt названия файлов, содержащихся в каталоге /etc. Допишите в этот же файл названия файлов, содержащихся в вашем домашнем каталоге.

![Рис.1: ](image/lab6.1.jpg){ #fig:001 width=70% }

## 2. Выведили имена всех файлов из file.txt, имеющих расширение .conf, после чего запишите их в новый текстовой файл conf.txt.

![Рис.2: ](image/lab6.2.jpg){ #fig:002 width=70% }

## 3. Определили, какие файлы в вашем домашнем каталоге имеют имена, начинавшиеся с символа c

![Рис.3: ](image/lab6.3.jpg){ #fig:003 width=70% }

## 4. Выведили на экран (по странично) имена файлов из каталога /etc, начинающиеся с символа h

![Рис.4: ](image/lab6.4.jpg){ #fig:004 width=70% }

## 5. Запустили в фоновом режиме процесс, который будет записывать в файл ~/logfile файлы, имена которых начинаются с log. Удалили файл ~/logfile.

![Рис.5: ](image/lab6.5.jpg){ #fig:005 width=70% }

## 6. Запустили из консоли в фоновом режиме редактор gedit. Определите идентификатор процесса gedit, используя команду ps, конвейер и фильтр grep.

![Рис.6: ](image/lab6.6.jpg){ #fig:006 width=70% }

## 7. Прочитали справку (man) команды kill, после чего используйте её для завершения процесса gedit

![Рис.7: ](image/lab6.7.jpg){ #fig:007 width=70% }

## 8. Выполнили команды df и du, предварительно получив более подробную информацию об этих командах, с помощью команды man.

![Рис.8: ](image/lab6.10.png){ #fig:008 width=70% }

## 9. Воспользовавшись справкой команды find, выведите имена всех директорий, имеющихся в вашем домашнем каталоге.

![Рис.9: ](image/lab6.8.jpg){ #fig:009 width=70% }
![Рис.10: ](image/lab6.9.jpg){ #fig:010 width=70% }

# Выводы

Ознакомились с инструментами поиска файлов и фильтрации текстовых данных. Приобретели практические навыки: по управлению процессами (и заданиями), по
проверке использования диска и обслуживанию файловых систем.

:::
