---
## Front matter
lang: ru-RU
title: "Первоначальна настройка git"
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

Изучить идеологию и применение средств контроля версий.
Освоить умения по работе с git.

# Задание

Создать базовую конфигурацию для работы с git.
Создать ключ SSH.
Создать ключ PGP.
Настроить подписи git.
Зарегистрироваться на Github.
Создать локальный каталог для выполнения заданий по предмету.

# Выполнение лабораторной работы

## Установка программного обеспечения

1. Установка git и gh

![Puc.1: Установим git и gh](image/lab2.1.jpg){ #fig:001 width=50%}

## Базовая настройка git

1. Зададим имя и email владельца репозитория:
2. Настроим utf-8 в выводе сообщений git:
3.Настройте верификацию и подписание коммитов git (см. Верификация коммитов git с помощью GPG).
  Зададим имя начальной ветки (будем называть её master):
4. Параметр autocrlf:
5. Параметр safecrlf:

![Puc.2: Базовая настройка git](image/lab2.2.jpg){ #fig:002 width=50%}

## Создание ключи ssh и pgp

1. по алгоритму rsa с ключём размером 4096 бит:
2. по алгоритму ed25519:
3. Генерируем ключ
4. Из предложенных опций выбираем:
	- тип RSA and RSA;
	- размер 4096;
	- выберите срок действия; значение по умолчанию — 0 (срок действия не истекает никогда).
5. GPG запросит личную информацию, которая сохранится в ключе:
	- Имя (не менее 5 символов).
	- Адрес электронной почты.
	- При вводе email убедитесь, что он соответствует адресу, используемому на GitHub.
	- Комментарий. Можно ввести что угодно или нажать клавишу ввода, чтобы оставить это поле пустым.

![Puc.3: Cоздание ключи pgp](image/lab2.3.jpg){ #fig:003 width=50%}
![Puc.4: Cоздание ключи pgp](image/lab2.4.jpg){ #fig:004 width=50%}

## Добавление PGP ключа в GitHub

1. Выводим список ключей и копируем отпечаток приватного ключа:
2. Cкопируйте ваш сгенерированный PGP ключ в буфер обмена:
3. Перейдите в настройки GitHub (https://github.com/settings/keys), нажмите на кнопку New GPG key и вставьте полученный ключ в поле ввода.

![Puc.5:](image/lab2.7.jpg){ #fig:005 width=50%}
![Puc.6:](image/lab2.8.jpg){ #fig:006 width=50%}
![Puc.7:](image/lab2.5.jpg){ #fig:007 width=50%}
![Puc.8:](image/lab2.6.jpg){ #fig:008 width=50%}

## Настройка автоматических подписей коммитов git

Используя введёный email, укажите Git применять его при подписи коммитов:

![Puc.9: Настройка автоматических подписей коммитов git](image/lab2.9.jpg){ #fig:009 width=50%}

## Настройка gh

![Puc.10: Авторизование](image/lab2.10.jpg){ #fig:010 width=50%}

## Шаблон для рабочего пространства

### Сознание репозитория курса на основе шаблона

![Puc.11: ](image/lab2.11.jpg){ #fig:011 width=50%}
![Puc.12: ](image/lab2.12.jpg){ #fig:012 width=50%}

### Настройка каталога курса

![Puc.13: ](image/lab2.14.jpg){ #fig:013 width=50%}

# Выводы

Мы приобрели практические навыки работы с git.

::: {#refs}
:::
