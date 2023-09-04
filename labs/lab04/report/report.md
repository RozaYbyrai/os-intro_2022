---
## Front matter
title: "Основы интерфейса взаимодействия
пользователя с системой Unix на уровне командной строки"
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

Приобретение практических навыков взаимодействия пользователя с системой посредством командной строки.

# Выполнение лабораторной работы

1. Определить полное имя домашнего каталога.

![Рис.1: Команды cd,pwd,ls](image/lab4.1.jpg){ #fig:001 width=70% }

2. Выполнение следующих действий:
	1. Переход в каталог /tmp.

	![Рис.2: ](image/lab4.2.jpg){ #fig:002 width=70% }

	2. Выведение на экран содержимое каталога /tmp. Для этого использовали команду ls
           с различными опциями. 

	![Рис.3: ](image/lab4.3.jpg){ #fig:003 width=70% }
	![Рис.4: ](image/lab4.4.jpg){ #fig:004 width=70% }
	![Рис.5: ](image/lab4.5.jpg){ #fig:005 width=70% }

	3. Определите, есть ли в каталоге /var/spool подкаталог с именем cron? Нет.
    
    	![Рис.6: ](image/lab4.6.jpg){ #fig:006 width=70% }
    
	4. Перейдите в Ваш домашний каталог и выведите на экран его содержимое. Определите, кто является владельцем файлов и подкаталогов?
 
	![Рис.8: ](image/lab4.8.jpg){ #fig:008 width=70% }
	![Рис.9: ](image/lab4.9.jpg){ #fig:009 width=70% }

3. Выполнение следующих действий:
	1. В домашнем каталоге создаем новый каталог с именем newdir. В каталоге ~/newdir создаем новый каталог с именем morefun.
    		В домашнем каталоге создаем одной командой три новых каталога с именами
		letters, memos, misk. Затем удалите эти каталоги одной командой. Попробуем удалить ранее созданный каталог ~/newdir командой rm. Проверим,
		был ли каталог удалён. Удалим каталог ~/newdir/morefun из домашнего каталога. Проверим, был ли
		каталог удалён.

	![Рис.10: ](image/lab4.10.jpg){ #fig:010 width=70% }
	![Рис.11: ](image/lab4.11.jpg){ #fig:011 width=70% }

4. . С помощью команды man определим, какую опцию команды ls нужно использовать для просмотра содержимое не только указанного каталога, но и подкаталогов,
входящих в него.	
	![Рис.13: ](image/lab4.13.jpg){ #fig:013 width=70% }

5. С помощью команды man определили набор опций команды ls, позволяющий отсортировать по времени последнего изменения выводимый список содержимого каталога
с развёрнутым описанием файлов.
	![Рис.14: ](image/lab4.14.jpg){ #fig:014 width=70% }

6. . Используя команду man для просмотра описания следующих команд: cd, pwd, mkdir,
rmdir, rm. Пояснили основные опции этих команд.

	![Рис.15: ](image/lab4.15.jpg){ #fig:015 width=70% }
	![Рис.16: ](image/lab4.16.jpg){ #fig:016 width=70% }
	![Рис.17: ](image/lab4.17.jpg){ #fig:017 width=70% }
	![Рис.18: ](image/lab4.18.jpg){ #fig:018 width=70% }
	![Рис.19: ](image/lab4.19.jpg){ #fig:019 width=70% }

7. Используя информацию, полученную при помощи команды history, выполнили модификацию и исполнение нескольких команд из буфера команд.
   
	![Рис.20: ](image/lab4.20.jpg){ #fig:020 width=70% }

# Выводы

Мы приобрели практические навыки взаимодействия пользователя с системой посредством командной строки.

:::
