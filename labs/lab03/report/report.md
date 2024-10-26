---
## Front matter
title: "Отчёт по лабораторной работе 3"
subtitle: "Архитектура компьютера"
author: "Чермашенцев Павел Андреевич НБИбд-03-24"

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

Целью данной работы является изучение процесса оформления отчетов с использованием легковесного языка разметки Markdown.

# Выполнение лабораторной работы

## Знакомство с Markdown

В соответствии с указаниями лабораторной работы, мы установили программы pandoc и TeX Live.

Открываю терминал и перехожу в каталог курса, созданный во время выполнения лабораторной работы №3. Затем обновляю локальный репозиторий, загрузив изменения из удаленного источника.

После этого, перехожу в каталог с шаблоном отчета для лабораторной работы №3.

Провожу компиляцию шаблона, используя Makefile. Для этого вводится команда `make`. При успешной компиляции должны быть сгенерированы файлы `report.pdf` и `report.docx`. Я открою их и проверю корректность полученных документов. (рис. [-@fig:001], [-@fig:002], [-@fig:003])

![Компиляция файлов](image/01.png){ #fig:001 width=70%, height=70% }

![Просмотр docx файла](image/02.png){ #fig:002 width=70%, height=70% }

![Просмотр pdf файла](image/03.png){ #fig:003 width=70%, height=70% }

Удаляю сгенерированные файлы, используя команду `make clean`. Это позволит убедиться, что после выполнения данной команды файлы `report.pdf` и `report.docx` были успешно удалены. (рис. [-@fig:004])

![Удаление файлов docx и pdf](image/04.png){ #fig:004 width=70%, height=70% }

Открываю файл `report.md` в текстовом редакторе, например, gedit. Внимательно изучаю структуру этого файла. (рис. [-@fig:005])

![Изучаю шаблон отчета](image/05.png){ #fig:005 width=70%, height=70% }

Заполняю отчет и компилирую его снова с использованием Makefile. Затем проверяю корректность сгенерированных файлов. (рис. [-@fig:006])

![Заполняю свой отчет](image/06.png){ #fig:006 width=70%, height=70% }

Загружаю готовые файлы на GitHub.

## Выполнение заданий для самостоятельной работы

Я подготовил отчет по лабораторной работе №2 и разместил его в репозитории. (рис. [-@fig:007], [-@fig:008])

![Заполняю отчет по лабораторной №2](image/07.png){ #fig:007 width=70%, height=70% }

![Компилирую отчет по лабораторной №2](image/08.png){ #fig:008 width=70%, height=70% }

# Выводы

В ходе выполнения данной лабораторной работы я изучил синтаксис языка разметки Markdown и научился генерировать отчеты из шаблонов с использованием Makefile, что значительно упростило процесс оформления документов.

