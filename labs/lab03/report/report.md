---
## Front matter
title: "Markdown"
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

Научиться оформлять отчёты с помощью легковесного языка разметки Markdown.

# Выполнение лабораторной работы
## Базовые сведения о Markdown

1. Чтобы создать заголовок, используйте знак ( # ), например:
 
![Рис.1: ](image/lab3.1.png){ #fig:001 width=40%}
![Рис.2: ](image/lab3.2.png){ #fig:002 width=40%}

2. Чтобы задать для текста полужирное начертание, заключите его в двойные звездочки:
   
![Рис.3: ](image/lab3.3.png){ #fig:003 width=40%}
![Рис.4: ](image/lab3.4.png){ #fig:004 width=40%}

3. Чтобы задать для текста курсивное начертание, заключите его в одинарные звездочки:

![Рис.5: ](image/lab3.5.png){ #fig:005 width=40%}
![Рис.6: ](image/lab3.6.png){ #fig:006 width=40%}

4. Чтобы задать для текста полужирное и курсивное начертание, заключите его в тройные
звездочки:

![Рис.7: ](image/lab3.7.png){ #fig:007 width=40%}
![Рис.8: ](image/lab3.8.png){ #fig:008 width=40%}

5. Блоки цитирования создаются с помощью символа >:

![Рис.9: ](image/lab3.9.png){ #fig:009 width=40%}
![Рис.10: ](image/lab3.10.png){ #fig:010 width=40%}

6. Неупорядоченный (маркированный) список можно отформатировать с помощью звездочек или тире:

![Рис.11: ](image/lab3.11.png){ #fig:011 width=40%}
![Рис.12: ](image/lab3.12.png){ #fig:012 width=40%}

7. Чтобы вложить один список в другой, добавьте отступ для элементов дочернего списка:

![Рис.13: ](image/lab3.13.png){ #fig:013 width=40%}
![Рис.14: ](image/lab3.14.png){ #fig:014 width=40%}

8. Упорядоченный список можно отформатировать с помощью соответствующих цифр:

![Рис.15: ](image/lab3.15.png){ #fig:015 width=40%}
![Рис.16: ](image/lab3.16.png){ #fig:016 width=40%}

9. Чтобы вложить один список в другой, добавьте отступ для элементов дочернего списка:

![Рис.17: ](image/lab3.17.png){ #fig:017 width=40%}
![Рис.18: ](image/lab3.18.png){ #fig:018 width=40%}

10. Синтаксис Markdown для встроенной ссылки состоит из части [link text] , представляющей текст гиперссылки, и части (file-name.md) – URL-адреса или имени файла,
на который дается ссылка:

![Рис.19: ](image/lab3.19.png){ #fig:019 width=40%}
![Рис.20: ](image/lab3.20.png){ #fig:020 width=40%}

11. Markdown поддерживает как встраивание фрагментов кода в предложение, так и их
размещение между предложениями в виде отдельных огражденных блоков. Огражденные
блоки кода — это простой способ выделить синтаксис для фрагментов кода. Общий
формат огражденных блоков кода:

![Рис.21: ](image/lab3.21.png){ #fig:021 width=40%}
![Рис.22: ](image/lab3.22.png){ #fig:022 width=40%}

12. Верхние и нижние индексы, внутритекстовые формулы делаются аналогично формулам LaTeX.:

![Рис.23: ](image/lab3.23.png){ #fig:023 width=40%}
![Рис.24: ](image/lab3.24.png){ #fig:024 width=40%}

13. Выключные формулы:
sin2
(𝑥) + cos2
(𝑥) = 1
{#eq:eq:sin2+cos2} со ссылкой в тексте «Смотри формулу ([-@eq:eq:sin2+cos2]).» записывается как

![Рис.25: ](image/lab3.25.png){ #fig:025 width=40%}
![Рис.26: ](image/lab3.26.png){ #fig:026 width=40%}

# Выводы

Научили базовые сведения о Markdown


::: {#refs}
:::
