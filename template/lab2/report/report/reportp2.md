---
## Front matter
title: "Лабораторная работа 2"
subtitle: "Компьютерный практикум по статистическому анализу данных"
author: "Ромицына Анастасия Романовна"

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

# Введение

Основная цель работы — изучить несколько структур данных, реализованных в Julia,
научиться применять их и операции над ними для решения задач.


# Выполнение лаборатаорной работы

Введем задание из лабораторной работы "Кортежи"
(рис. [-@fig:001]).

![Кортежи](image/1.png){#fig:001 width=40%}

Введем задание из лабораторной работы "Словари" .(рис. [-@fig:002]).

![Словари](image/2.png){#fig:002 width=40%}

Введем задание из лабораторной работы "Множества"
 (рис. [-@fig:003]).

![Множества](image/3.png){#fig:003 width=40%}

Введем задание из лабораторной работы "Массивы" (рис. [-@fig:004]).

![Массивы](image/4.png){#fig:004 width=40%}

Введем задание из лабораторной работы "Массивы"
(рис. [-@fig:005]).

![Массивы](image/5.png){#fig:005 width=40%}

Введем задание из лабораторной работы "Массивы" (рис. [-@fig:006]).

![Массивы](image/6.png){#fig:006 width=40%}

Введем задание из лабораторной работы "Массивы" (рис. [-@fig:007]).

![Массивы](image/7.png){#fig:007 width=40%}

Введем задание из лабораторной работы "Массивы" (рис. [-@fig:008]).

![Массивы](image/8.png){#fig:008 width=40%}

Введем задание из лабораторной работы "Массивы" (рис. [-@fig:009]).

![Массивы](image/9.png){#fig:009 width=40%}

Решим задание 1 и 2 из лабораторной работы
𝑃 = 𝐴 ∩ 𝐵 ∪ 𝐴 ∩ 𝐵 ∪ 𝐴 ∩ 𝐶 ∪ 𝐵 ∩ 𝐶. (рис. [-@fig:010]).

![Задание 1,2](image/10.png){#fig:010 width=40%}

Решим задание 3.1-3.9 с разными видами массивов из лабораторной работы(рис. [-@fig:011]).

![Задание 3.1-3.9](image/11.png){#fig:011 width=40%}

Решим задание 3.10-3.13 с разными видами массивов из лабораторной работы(рис. [-@fig:012]).

![Задание 3.10-3.13](image/12.png){#fig:012 width=40%}


Решим задание 3.14 с разными видами массивов из лабораторной работы(рис. [-@fig:013]).

![Задание 3.14](image/13.png){#fig:013 width=40%}

Решим задание 4 с разными видами массивов из лабораторной работы(рис. [-@fig:014]).

![Задание 4](image/14.png){#fig:014 width=40%}

Решим задание 5 и 6 с разными видами массивов из лабораторной работы(рис. [-@fig:015]).

![Задание 5 и 6 ](image/15.png){#fig:015 width=40%}

# Вывод

Мы смогли изучить несколько структур данных, реализованных в Julia,
научиться применять их и операции над ними для решения задач.

# Список литературы{.unnumbered}

::: {#refs}
:::
