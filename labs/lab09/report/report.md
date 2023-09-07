---
## Front matter
title: "Текстовой редактор emacs"
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

Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором Emacs.

# Задание

Научиться работать с редактором emacs.

# Выполнение лабораторной работы
## Основные команды emacs
1. Открывание emacs

![Рис.1: открывание emacs](image/lab9.1.jpg){ #fig:001 width=70% }

2. Создавание файла

![Рис.2: создавание файла](image/lab9.2.jpg){ #fig:002 width=70% }

3. Написать текст в файл

![Рис.3: ](image/lab9.3.jpg){ #fig:003 width=70% }


4. Сохранение файла
   
![Рис.4: сохранение файла](image/lab9.4.jpg){ #fig:004 width=70% }

5. Проделать с текстом стандартные процедуры редактирования, каждое действие должно осуществляться комбинацией клавиш.
	- Вырезать одной командой целую строку (С-k).
	- Вставить эту строку в конец файла (C-y).
	- Выделить область текста (C-space).
	- Скопировать область в буфер обмена (M-w).
	- Вставить область в конец файла.
	- Вновь выделить эту область и на этот раз вырезать её (C-w).
	- Отмените последнее действие (C-/).
   	- Научитесь использовать команды по перемещению курсора.
	- Переместите курсор в начало строки (C-a).
	- Переместите курсор в конец строки (C-e).
	- Переместите курсор в начало буфера (M-<).
	- Переместите курсор в конец буфера (M->).

![Рис.5: ](image/lab9.5.jpg){ #fig:005 width=70% }

![Рис.6: ](image/lab9.6.jpg){ #fig:006 width=70% }

![Рис.7: ](image/lab9.7.jpg){ #fig:007 width=70% }

![Рис.8: ](image/lab9.8.jpg){ #fig:008 width=70% }

6. Вывести список активных буферов на экран (C-x C-b).Переместитесь во вновь открытое окно (C-x) o со списком открытых буферов
и переключитесь на другой буфер. Закройте это окно (C-x 0). Теперь вновь переключайтесь между буферами, но уже без вывода их списка наэкран (C-x b).

![Рис.9:выведение список ](image/lab9.9.jpg){ #fig:009 width=70% }

![Рис.10: перемещение](image/lab9.10.jpg){ #fig:010 width=70% }

![Рис.11: закрывание](image/lab9.11.jpg){ #fig:011 width=70% }

![Рис.12: ](image/lab9.12.jpg){ #fig:012 width=70% }

7. Поделить фрейм на 4 части: разделите фрейм на два окна по вертикали (C-x 3), а затем каждое из этих окон на две части по горизонтали (C-x 2) 

![Рис.13: поделение фрейм на 4 части](image/lab9.13.jpg){ #fig:013 width=70% }

8. В каждом из четырёх созданных окон открыть новый буфер (файл) и ввести несколько строк текста.

![Рис.14: открывание буфер и введение строк](image/lab9.14.jpg){ #fig:014 width=70% }

9. Переключитесь в режим поиска (C-s) и найдите несколько слов, присутствующих в тексте.

![Рис.15: найти слов из текста](image/lab9.15.jpg){ #fig:015 width=70% }

10. Переключайтесь между результатами поиска, нажимая C-s
    
![Рис.16: Переключение между поисков](image/lab9.16.jpg){ #fig:016 width=70% }

11. Выйти из режима нажав на C-g.
    
# Выводы

В ходе данной лабораторной работы научились работать с текстовым редактором emacs.

:::
