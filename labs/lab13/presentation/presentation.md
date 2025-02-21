---
## Front matter
lang: ru-RU
title: Лабораторная работа №13
subtitle: Операционные системы
author:
  - Александрова Ульяна
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 06 мая 2023

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---

# Информация

## Докладчик


  * Александрова Ульяна
  * студентка 1-го курса
  * Российский университет дружбы народов
  * [kulyabov-ds@rudn.ru](mailto:1132226444@pfur.ru)
  * <https://AleksandrovaUV.github.io/ru/>


# Цель работы

## Цель работы

Приобрести простейшие навыки разработки, анализа, тестирования и отладки приложений в ОС типа UNIX/Linux на примере создания на языке программирования
С калькулятора с простейшими функциями.

# Задание

## Задание

1. В домашнем каталоге создайте подкаталог ~/work/os/lab_prog.
2. Создайте в нём файлы: calculate.h, calculate.c, main.c. Это будет примитивнейший калькулятор, способный складывать, вычитать, умножать и делить, возводить число в степень, брать квадратный корень, вычислять sin, cos, tan. При запуске он будет запрашивать первое число, операцию, второе число. После этого программа выведет результат и остановится.
3. Выполните компиляцию программы посредством gcc.
4. При необходимости исправьте синтаксические ошибки.
5. Создайте Makefile со следующим содержанием.
6. С помощью gdb выполните отладку программы calcul (перед использованием gdb исправьте Makefile).
7. С помощью утилиты splint попробуйте проанализировать коды файлов calculate.c и main.c.

# Выполнение лабораторной работы

## Выполнение лабораторной работы

Создала требуемый репозиторий и файлы, необходимые для выполнения работы.

![Создание файлов](image/1.png){#fig:001 width=70%}

## Выполнение лабораторной работы

Записываю реализацию функций калькулятора сначала в файле calculate.h.

![calculate.h](image/2.png){#fig:002 width=70%}

## Выполнение лабораторной работы

Затем в calculate.c.

![calculate.c](image/3.png){#fig:003 width=70%}

## Выполнение лабораторной работы

И в main.c.

![main.c](image/4.png){#fig:004 width=70%}

## Выполнение лабораторной работы

Выполняю компиляцию программы посредством gcc.

![Компиляция](image/5.png){#fig:005 width=70%}

## Выполнение лабораторной работы

Создаю и заполняю файл Makefile.

![Makefile](image/9.png){#fig:006 width=70%}

## Выполнение лабораторной работы

Запустила отладчик gdb, программа работает.

![Отладка](image/6.png){#fig:007 width=70%}

## Выполнение лабораторной работы

Для постраничного просмотра исходного код использовала команду list.

![Просмотр кода](image/7.png){#fig:008 width=70%}

# Выводы

## Вывод

Я приобрела простейшие навыки разработки, анализа, тестирования и отладки приложений в ОС типа UNIX/Linux на примере создания на языке программирования С калькулятора с простейшими функциями.


