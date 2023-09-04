---
## Front matter
title: "Установка ОС Linux на виртуальную машину"
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

Целью данной работы является приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

# Задание

Создать виртуальную машину и на ней установить операционную систему.


# Выполнение лабораторной работы
## Процесс создания виртуальной машины
1. Укажем имя и тип ОС виртуальной машины
![Рис.1: Имя и тип ОС ВМ](image/lab1.1.png){ #fig:001 width=50% }

2. Создаём новый виртуальный жесткий диск и задаём размер диска
![Рис.2: Создание диска](image/lab1.2.png){ #fig:002 width=50% }

3. Укажем размер основной памяти виртуальной машины — от 2048 МБ.
![Рис.3: Размер основной памяти ВМ](image/lab1.3.png){ #fig:003 width=50% }

4. Итог
   
![Рис.4: Итог](image/lab1.4.png){ #fig:004 width=50% }

### Установка ОС

5. Установка языка
![Рис.5: Установка языка](image/lab1.5.png){ #fig:005 width=50% }

6. Региональные настройки система
![Рис.6: Региональные настройки система](image/lab1.6.png){ #fig:006 width=50% }

7. Завершение установки
![Рис.7: Завершение установки](image/lab1.7.png){ #fig:007 width=50% }

8. Установка имени и пароля для пользователя root
![Рис.8: Установка имени и пароля для пользователя root](image/lab1.8.png){ #fig:008 width=50% }

9. Установка дополнений гостевой ОС

![Рис.9: Установка дополнений гостевой ОС](image/lab1.9.jpg){ #fig:009 width=50% }

#### Обновления

10. Обновление всех пакетов

![Рис.10: Обновления пакетов](image/lab1.10.jpg){ #fig:010 width=50% }

11. Установка драйверов для VirtualBox
    
![Рис.11: Установка драйверов](image/lab1.11.jpg){ #fig:011 width=50% }
![Рис.12: Установка драйверов](image/lab1.12.jpg){ #fig:012 width=50% }

12. Настройка раскладки клавиатуры

![Рис.13: Настройка раскладки клавиатуры](image/lab1.13.jpg){ #fig:013 width=50% }

13. Установка имени пользователя и названия хоста

![Рис.14: Установка имени пользователя и названия хоста](image/lab1.14.jpg){ #fig:014 width=50% }
![Рис.15: Установка имени пользователя и названия хоста](image/lab1.15.jpg){ #fig:015 width=50% }

14. pandoc

![Рис.16: pandoc](image/lab1.16.jpg){ #fig:016 width=50% }
![Рис.17: pandoc](image/lab1.17.jpg){ #fig:017 width=50% }

15. texlive

![Рис.18: texlive](image/lab1.18.jpg){ #fig:018 width=50% }

# Выводы

Мы приобрели практические навыки установки операционных систем на виртуальную машину и настройки минимально необходимых для дальнейшей работы сервисов.

