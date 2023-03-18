---
## Front matter
title: "Отчет по 2-ому этапу проекта"
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

Добавление к сайту данные о себе.

# Задание

* Разместить фотографию владельца сайта.
* Разместить краткое описание владельца сайта (Biography).
* Добавить информацию об интересах (Interests).
* Добавить информацию от образовании (Education).
* Сделать пост по прошедшей неделе.
* Добавить пост на тему: Управление версиями. Git.

# Выполнение проекта

Я изменила шаблон в файле проекта blog_UV/content/author/admin/_index.md в соответствии с данными о себе и заданием (рис. @fig:001).

![Изменение шаблона сайта](image/1){#fig:001 width=70%}

Далее использовала утилиту hugo и git add, чтобы загрузить изменения на сервер. Изменения успешно применены (рис. @fig:002).

![Применение](image/2){#fig:002 width=70%}

Проделала схожие изменения над шаблоном в папке blog_UV/content/post/getting-started, чтобы создать новый пост на сайте, и так же загрузила его на сервер (рис. @fig:003) (рис. @fig:004).

![Изменение шаблона поста](image/3){#fig:003 width=70%}

![Созданный пост](image/4){#fig:004 width=70%}

Создала новый пост о предложенной тебе и загрузила его на сервер (рис. @fig:005).

![Новый пост по теме задания](image/5){#fig:005 width=70%}

# Выводы

Я научилась изменять информацию о себе и создавать посты.


::: {#refs}
:::
