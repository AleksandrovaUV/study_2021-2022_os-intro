---
## Front matter
title: "Лабораторная работа №8"
subtitle: "Операционные системы"
author: "Александрова Ульяна"

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

Целью работы является ознакомление с операционной системой Linux и получение практических навыки работы с редактором vi, установленным по умолчанию практически во всех дистрибутивах.

# Задание

1. Ознакомиться с теоретическим материалом.
2. Ознакомиться с редактором vi.
3. Выполнить упражнения, используя команды vi.

# Теоретическое введение

В большинстве дистрибутивов Linux в качестве текстового редактора по умолчанию
устанавливается интерактивный экранный редактор vi (Visual display editor).

Редактор vi имеет три режима работы:
- командный режим — предназначен для ввода команд редактирования и навигации по
редактируемому файлу;
- режим вставки — предназначен для ввода содержания редактируемого файла;
- режим последней (или командной) строки — используется для записи изменений в файл и выхода из редактора.

Для вызова редактора vi необходимо указать команду vi и имя редактируемого файла: vi <имя_файла>  
При этом в случае отсутствия файла с указанным именем будет создан такой файл.

Переход в командный режим осуществляется нажатием клавиши Esc. Для выхода из редактора vi необходимо перейти в режим последней строки: находясь в командном режиме, нажать Shift-; (по сути символ : — двоеточие), затем:
- набрать символы wq, если перед выходом из редактора требуется записать изменения
в файл;
- набрать символ q (или q!), если требуется выйти из редактора без сохранения.

# Выполнение лабораторной работы

Я создала каталог в папке os-intro с именем lab06, а также вызвала vi и создала файл hello.sh (рис. @fig:001).

![Запуск редактора](image/1.PNG){#fig:001 width=70%}

Нажав клавишу i, ввела предложенный текст (рис. @fig:002).

![Ввод текста](image/2.PNG){#fig:002 width=70%}

Перешла в командный режим, затем вызвала :, записала и вышла из редактора (рис. @fig:003).

![:wq](image/3.PNG){#fig:003 width=70%}

Сделала файл исполняемым (рис. @fig:004).

![Исполнение файла](image/4.PNG){#fig:004 width=70%}

Вызвала vi и заменила HELL во второй строке на HELLO, вернулась в командный режим (рис. @fig:005).

![Изменения 1](image/5.PNG){#fig:005 width=70%}

Стерла в четвертой строчке LOCAL и заменила на local (рис. @fig:006).

![Изменения 2](image/6.PNG){#fig:006 width=70%}

Удалила последнюю строки и отменила изменения. Вышла из редактора (рис. @fig:007).

![Изменения 3](image/7.PNG){#fig:007 width=70%}

# Выводы

Я ознакомилась с операционной системой Linux и полученила практические навыки работы с редактором vi, установленным по умолчанию практически во всех дистрибутивах.

::: {#refs}
:::
