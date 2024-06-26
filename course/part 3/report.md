---
## Front matter
title: "Отчёт прохождения внешнего курса"
subtitle: "Безопасность в сети"
author: "Криптография на практике"

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

Провести контроль усвоения теоритического материала раздела "Криптография на практике"

# Выполнение контрольных заданий

В асимметричной криптографии, также известной как криптография с открытым ключом, каждая сторона обладает парой ключей: открытым и закрытым (или секретным). Открытый ключ доступен для общего использования, в то время как закрытый ключ хранится конфиденциально у владельца. К протоколам асимметричной криптографии относятся электронно-цифровая подпись и протокол генерации общего ключа. Последний позволяет установить общий секретный ключ без необходимости физического взаимодействия между сторонами.(рис. [-@fig:001]).

![Задание 1](image/image1.png){#fig:001 width=70%}

Криптографическая хэш-функция, эффективно вычисляется, дает на выходе фиксированное число бит независимо от объема входных данных, но главное она стойкая к колизиям. Это значит что двое разных входных данных не могут дать один выходной(рис. [-@fig:002]).

![Задание 2](image/image2.png){#fig:002 width=70%}

К ним относятся именно RSA, ECDSA, ГОСТ Р 34.10-2012, остальные отношения не имеют(рис. [-@fig:003]).

![Задание 3](image/image3.png){#fig:003 width=70%}

Этот процесс также является симметричным и использует ключ (который должен быть отличным от ключа, использованного для шифрования) и само сообщение для создания кода аутентификации. Этот примитив можно представить как симметричный аналог подписи. Обычно код аутентификации сообщения создается с использованием хэш-функции или симметричного шифрования.(рис. [-@fig:004]).

![Задание 4](image/image4.png){#fig:004 width=70%}

Обмен ключам Диффи-Хэллмана - это асимметричный примитив генерации общего секретного ключа(рис. [-@fig:005]).

![Задание 5](image/image5.png){#fig:005 width=70%}

Конечно же к протоколам с публичным(открытым ключом)(рис. [-@fig:006]).

![Задание 6](image/image6.png){#fig:006 width=70%}

НАм в первую очередь нужна сама подпись, потом открытый ключ(никак не секретный) и потом также сообщение. ТОлько так пройдёт верификация (рис. [-@fig:007]).

![Задание 7](image/image7.png){#fig:007 width=70%}

Конечно конфиденциальность. Это же подпись. ОНа указывает на человека, которому принадлежит(рис. [-@fig:008]).

![Задание 8](image/image8.png){#fig:008 width=70%}

Только усиленная квалифицированная. Это касается серьёзных документов. Никакая другая не подойдёт (рис. [-@fig:009]).

![Задание 9](image/image9.png){#fig:009 width=70%}

Только в удостоверяющем, сертификационном центре. Иные организации таких полномочий не имеют.(рис. [-@fig:010]).

![Задание 10](image/image10.png){#fig:010 width=70%}

Мастеркарт и мир. Биткоин это валюта, банкомат - усстройство, выдающее и принимающе деньги.(рис. [-@fig:011]).

![Задание 11](image/image11.png){#fig:011 width=70%}

Нам нужны доказательства из разных категорий. Минимум две. В эти категории входят наша биометрия, то что мы знаем(пароль) и то что имеем (наприер телефон). Пароль и капча таковыми не являются, капча это вообще защита от автоматических атак, ну и пин код с паролем тоже из одной категории(рис. [-@fig:012]).

![Задание 12](image/image12.png){#fig:012 width=70%}

При онлайн платежах сегодня используется многофакторная аутентификация покупателя перед банком-эмитентом(рис. [-@fig:013]).

![Задание 13](image/image13.png){#fig:013 width=70%}

СЛожность нахождения прообраза конечно же. Это очень важное свойствр(рис. [-@fig:014]).

![Задание 14](image/image14.png){#fig:014 width=70%}

Снова задание с подвохом. ЗДесь подходят все варианты. Об этом говорилось в лекции(рис. [-@fig:015]).

![Задание 15](image/image15.png){#fig:015 width=70%}

(рис. [-@fig:016]).

![Задание 16](image/image16.png){#fig:016 width=70%}

# Выводы

Мы успешно прошли контроль усвоения теоритического материала раздела "Криптография на практике"

# Список литературы{.unnumbered}

::: {#refs}
:::
