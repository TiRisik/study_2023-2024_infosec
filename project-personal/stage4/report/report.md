---
## Front matter
title: "Отчёт по четвёртому этапу индивидуального прокта"
subtitle: "Использование nikto"
author: "Тарутина Кристина Олеговна"

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

Научиться использовать базовый сканер безопасности веб-сервера nikto

# Выполнение лабораторной работы

Получаем справку по работе nikto (рис. [-@fig:001]).

nikto -h

![Справка](image/image1.png){#fig:001 width=70%}

Далее для примера запустим сканирование всем известного сайта github.com на пример уязвимостей(рис. [-@fig:002]).

nikto -h github.com

![Результат для github.com](image/image2.png){#fig:002 width=70%}

И теперь отcканируем собственную локальную сеть(рис. [-@fig:003]).

nikto -h 127.0.0.1

![Результат для локальной сети](image/image3.png){#fig:003 width=70%}


# Выводы

Мы успешно изучили базовый сканер безопасности веб-сервера nikto

# Список литературы{.unnumbered}

::: {#refs}
:::
