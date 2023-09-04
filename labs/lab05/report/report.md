---
## Front matter
title: "Анализ файловой системы Linux.Команды для работы с файлами и каталогами"
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

Ознакомление с файловой системой Linux, её структурой, именами и содержанием каталогов. Приобретение практических навыков по применению команд для работы
с файлами и каталогами, по управлению процессами (и работами), по проверке использования диска и обслуживанию файловой системы.

# Выполнение лабораторной работы

## Выполнение всех пример, приведённых в первой части описания лабораторной работы
1. Копирование файлов и каталогов
 
![Рис.1: ](image/lab5.1.jpg){ #fig:001 width=70% }

2. Перемещение и переименование файлов и каталогов

![Рис.2: ](image/lab5.2.jpg){ #fig:002 width=70% }

3. Права доступа

![Рис.3: ](image/lab5.3.jpg){ #fig:003 width=70% }
## Выполнение следующих действий

1. Скопирование файла /usr/include/sys/io.h в домашний каталог и назовим его equipment. Если файла io.h нет, то используем любой другой файл в каталоге
/usr/include/sys/ вместо него. В домашнем каталоге создаем директорию ~/ski.plases. Переместим файл equipment в каталог ~/ski.plases.
Переименуем файл ~/ski.plases/equipment в ~/ski.plases/equiplist. Создаем в домашнем каталоге файл abc1 и скопируйте его в каталог
~/ski.plases, назовем его equiplist2. Создаем каталог с именем equipment в каталоге ~/ski.plases. Переместим файлы ~/ski.plases/equiplist и equiplist2 в каталог ~/ski.plases/equipment. Создаем и переместите каталог ~/newdir в каталог ~/ski.plases и назовите его plans.

![Рис.4: ](image/lab5.4.jpg){ #fig:004 width=70% }

 2. Определим опции команды chmod, необходимые для того, чтобы присвоить перечисленным ниже файлам выделенные права доступа, считая, что в начале таких прав
нет:
	- drwxr--r-- ... australia
	- drwx--x--x ... play
	- -r-xr--r-- ... my_os
	- -rw-rw-r-- ... feathers

![Рис.5: ](image/lab5.5.jpg){ #fig:005 width=70% }

3.
	- Просмотрим содержимое файла /etc/password.
	- Скопируем файл ~/feathers в файл ~/file.old.
	- Переместим файл ~/file.old в каталог ~/play.
	- Скопируем каталог ~/play в каталог ~/fun.
	- Переместим каталог ~/fun в каталог ~/play и назовите его games.
	- Лишим владельца файла ~/feathers права на чтение.
	- Что произойдёт, если вы попытаетесь просмотреть файл ~/feathers командой cat? Отказано в доступе.
	- Что произойдёт, если вы попытаетесь скопировать файл ~/feathers? Отказано в доступе.
	- Даем владельцу файла ~/feathers право на чтение.
	- Лишим владельца каталога ~/play права на выполнение.
	- Перейдем в каталог ~/play. Что произошло?
	- Даем владельцу каталога ~/play право на выполнение.

 	![Рис.6: ](image/lab5.6.jpg){ #fig:006 width=70% }
	![Рис.7: ](image/lab5.7.jpg){ #fig:007 width=70% }
	
4. Прочтение man по командам mount, fsck, mkfs, kill
   	![Рис.8: ](image/lab5.8.jpg){ #fig:008 width=70% }
	![Рис.9: ](image/lab5.9.jpg){ #fig:009 width=70% }
	![Рис.10: ](image/lab5.10jpg){ #fig:010 width=70% }
	![Рис.11: ](image/lab5.11.jpg){ #fig:011 width=70% }
	![Рис.12: ](image/lab5.12.jpg){ #fig:012 width=70% }
# Выводы

В ходе выполнения данной работы мы ознакомились с файловой системой Linux, её структурой, именами и содержанием каталогов. Приобрели практические навыки по применению команд для работы с файлами и каталогами, по управлению процессами (и работами), по проверке использования диска и обслуживанию файловой системы.

:::
