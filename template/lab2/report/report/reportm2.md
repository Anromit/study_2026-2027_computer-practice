---
## Front matter
title: "Лабораторная работа 2"
subtitle: "Измерение и тестирование пропускной способности сети. Интерактивный эксперимент "
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

Основной целью работы является знакомство с инструментом для измерения
пропускной способности сети в режиме реального времени — iPerf3, а также
получение навыков проведения интерактивного эксперимента по измерению
пропускной способности моделируемой сети в среде Mininet.



# Выполнение лаборатаорной работы

Запустим виртуальную среду с minine
(рис. [-@fig:001]).

![Запуск виртуальной машины](image/1.png){#fig:001 width=70%}

Из основной ОС подключаемся к виртуальной машине.(рис. [-@fig:002]).

![Подключение](image/2.png){#fig:002 width=70%}

После подключения к виртуальной машине mininet посмотрим IP-адреса машины
 (рис. [-@fig:003]).

![Просмотр  IP-адреса](image/3.png){#fig:003 width=70%}

Активируем второй интерфейс, набрав в командной строке: (рис. [-@fig:004]).

![Активация интерфейса](image/4.png){#fig:004 width=70%}

Обновим репозитории программного обеспечения на виртуальной машине
(рис. [-@fig:005]).

![Репозитории](image/5.png){#fig:005 width=70%}

Установим iperf3 (рис. [-@fig:006]).

![Установка](image/6.png){#fig:006 width=70%}

Установим необходимое дополнительное программное обеспечение на виртуальную машину (рис. [-@fig:007]).

![Установка](image/7.png){#fig:007 width=70%}

Перейдем во временный каталог и скачаем репозиторий (рис. [-@fig:008]).

![Скачивание с git](image/8.png){#fig:008 width=70%}

Установим iperf3_plotter (рис. [-@fig:009]).

![Установка](image/9.png){#fig:009 width=100%}

Зададим простейшую топологию, состоящую из двух хостов и коммутатора
с назначенной по умолчанию mininet сетью 10.0.0.0/8 (рис. [-@fig:010]).

![Простейшая топология](image/10.png){#fig:010 width=100%}

В терминале виртуальной машины посмотрим параметры запущенной в интерактивном режиме топологии(рис. [-@fig:011]).

![Просмотр](image/11.png){#fig:011 width=70%}

В терминале h2 запустим сервер iPerf3 (рис. [-@fig:012]).

![Запуск сервера](image/12.png){#fig:012 width=100%}

В терминале хоста h1 запустим клиент iPerf3 (рис. [-@fig:013]).

![Запуск клиента](image/13.png){#fig:013 width=100%}

Запустим сервер iPerf3 на хосте h2 (рис. [-@fig:014]).

![Запуск сервера](image/14.png){#fig:014 width=100%}

Запустим клиент iPerf3 на хосте h1(рис. [-@fig:015]).

![Запуск клиента](image/15.png){#fig:015 width=100%}

Остановим серверный процесс (рис. [-@fig:016]).

![Остановка](image/16.png){#fig:016 width=100%}

В терминале h2 запустим сервер iPerf3. В терминале h1 запустим клиент iPerf3 с параметром -t, за которым
следует количество секунд (рис. [-@fig:017]).

![Запуск сервера и клиента](image/17.png){#fig:7 width=100%}

Настроим клиент iPerf3 для выполнения теста пропускной способности
с 2-секундным интервалом времени отсчёта как на клиенте, так и на сервере. (рис. [-@fig:018]).

![Настройка](image/18.png){#fig:018 width=100%}

Зададим на клиенте iPerf3 отправку определённого объёма данных (рис. [-@fig:019]).

![Настройка](image/19.png){#fig:019 width=100%}

Изменим в тесте измерения пропускной способности iPerf3 протокол передачи данных с TCP  на UDP(рис. [-@fig:020]).

![Изменение пропускной способности](image/20.png){#fig:020 width=100%}

В тесте измерения пропускной способности iPerf3 изменим номер порта для отправки/получения пакетов или датаграмм через указанный порт.(рис. [-@fig:021]).

![Настройка](image/21.png){#fig:021 width=100%}

В тесте измерения пропускной способности iPerf3 зададим
для сервера параметр обработки данных только от одного клиента с остановкой сервера по завершении теста (рис. [-@fig:022]).

![Настройка](image/22.png){#fig:022 width=100%}

В виртуальной машине mininet создадим каталог для работы над проектом(рис. [-@fig:023]).

![Создание каталога](image/23.png){#fig:023 width=100%}

Запустим клиент iPerf3 на хосте h1(рис. [-@fig:024]).

![В терминале h2 запустим сервер iPerf3](image/24.png){#fig:024 width=100%}

В терминале h1 запустим клиент iPerf3, указав параметр -J для отображения вывода результатов в формате JSON (рис. [-@fig:025]).

![Запуск клиента](image/25.png){#fig:025 width=100%}

Экспортируем вывод результатов теста в файл, перенаправив стандартный вывод в файл(рис. [-@fig:026]).

![Настройка](image/26.png){#fig:026 width=100%}

Убедимся, что файл iperf_results.json создан в указанном каталоге(рис. [-@fig:027]).

![Проверка](image/27.png){#fig:027 width=100%}

 В виртуальной машине mininet исправьте права запуска X-соединения (рис. [-@fig:028]).

![Исправление прав](image/28.png){#fig:028 width=100%}

В виртуальной машине mininet перейдем в каталог для работы над проектом, проверем права доступа
к файлу JSON(рис. [-@fig:029]).

![Проверка](image/29.png){#fig:029 width=100%}

Убедимся, что файлы с данными и графиками сформировались(рис. [-@fig:030]).

![Проверка](image/30.png){#fig:030 width=100%}

# Вывод

Мы смогли  познакомиться с инструментом для измерения
пропускной способности сети в режиме реального времени — iPerf3, а также
получили навыки проведения интерактивного эксперимента по измерению
пропускной способности моделируемой сети в среде Mininet.

# Список литературы{.unnumbered}

::: {#refs}
:::
