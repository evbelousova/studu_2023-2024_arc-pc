---
## Front matter
title: "Отчет по лабораторной работе №3"
subtitle: "Дисциплина: Архитектура компьютера"
author: "Белоусова Елизавета Валетиновна"

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

Целью данной лабораторной работы является освоение процедуры оформле-
ния отчетов с помощью легковесного языка разметки Markdown.
# Задание

1. Заполнение отчета по выполнению лабораторной работы №3 в формате Markdown
2. Выполнение заданий для самостоятельной работы
# Теоретическое введение

Markdown - легковесный язык разметки, созданный с целью обозначения фор-
матирования в простом тексте, с максимальным сохранением его читаемости
человеком, и пригодный для машинного преобразования в языки для продви-
нутых публикаций. Внутритекстовые формулы делаются аналогично формулам
LaTeX. В Markdown вставить изображение в документ можно с помощью непосред-
ственного указания адреса изображения. Синтаксис Markdown для встроенной
ссылки состоит из части [link text], представляющей текст гиперссылки, и ча-
сти (file-name.md) – URL-адреса или имени файла, на который дается ссылка.
Markdown поддерживает как встраивание фрагментов кода в предложение, так
и их размещение между предложениями в виде отдельных огражденных бло-
ков. Огражденные блоки кода — это простой способ выделить синтаксис для
фрагментов кода.

# Выполнение лабораторной работы

1. Открываю терминал. Перехожу в каталог курса, сформированный при выпол-
неннии прошлой лаборатной работы(рис. [-@fig:001])
![Перемещение между директориями](/afs/.dk.sci.pfu.edu.ru/home/e/v/evbelousova/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab03/report/image/Снимок экрана от 2023-10-13 12-20-20.png){#fig:001 width=70%}
Обновляю локальный репозиторий, скачав изменения из удаленного репози-
тория с помощью команды git pull (рис.[-@fig:002] )
![Обновление локального репозитория](/afs/.dk.sci.pfu.edu.ru/home/e/v/evbelousova/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab03/report/image/Снимок экрана от 2023-10-13 12-20-52.png){#fig:002 width=70%}
Перехожу в каталог с шаблоном отчета по лабораторной работе №3 с помощью
cd (рис.[-@fig:003] )
![Перемещение между директориями](/afs/.dk.sci.pfu.edu.ru/home/e/v/evbelousova/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab03/report/image/Снимок экрана от 2023-10-13 12-22-19.png){#fig:003 width=70%}
Компилирую шаблон с использованием Makefile, вводя команду make(рис.[-@fig:004] )
![Компиляция шаблона](/afs/.dk.sci.pfu.edu.ru/home/e/v/evbelousova/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab03/report/image/Снимок экрана от 2023-10-13 18-53-14.png){#fig:004 width=70%}
Удаляю полученные файлы с использованием Makefile, вводя команду make
clean(рис.[-@fig:005] )
![Удаление файлов](/afs/.dk.sci.pfu.edu.ru/home/e/v/evbelousova/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab03/report/image/Снимок экрана от 2023-10-13 19-03-53.png){#fig:005 width=70%}
С помощью команды ls проверяю, удалились ли созданные
файлы (рис.[-@fig:006] )
![Содержимое файла](/afs/.dk.sci.pfu.edu.ru/home/e/v/evbelousova/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab03/report/image/Снимок экрана от 2023-10-13 19-04-10.png){#fig:006 width=70%}
Открываю файл report.md с помощью текстового редактора gedit (рис.[-@fig:007] )
![Открытие файла rm](/afs/.dk.sci.pfu.edu.ru/home/e/v/evbelousova/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab03/report/image/Снимок экрана от 2023-10-13 19-05-32.png){#fig:007 width=70%}
Начинаю заполнять отчет с помощью языка разметки Markdown в скопирован-
ном файле. (рис.[-@fig:008] )
![Заполнение отчета](/afs/.dk.sci.pfu.edu.ru/home/e/v/evbelousova/work/study/2023-2024/Архитектура компьютера/arch-pc/labs/lab03/report/image/Снимок экрана от 2023-10-13 19-54-58.png){#fig:008 width=70%}
Компилирую файл с отчетом. Загружаю отчет на GitHub.
2. Задания для самостоятельной работы




# Выводы

Здесь кратко описываются итоги проделанной работы.

# Список литературы{.unnumbered}

::: {#refs}
:::
