---
# Front matter
lang: ru-RU
title: "Лабораторная работа 11"
subtitle: " Программирование в командном процессоре ОС UNIX. Ветвления и циклы"
author: "Шеожев Аслан Аскерович"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Отчет по лабораторной работе №11.
### Работу выполнил Шеожев Аслан Аскерович. 

## Цель работы:

Изучить основы программирования в оболочке ОС UNIX. Научится писать более сложные командные файлы с использованием логических управляющих конструкций и циклов.

## Ход работы:
1. Используя команды getopts grep, написал командный файл, который анализирует командную строку с ключами:

* -iinputfile — прочитать данные из указанного файла;
* -ooutputfile — вывести данные в указанный файл;
* -pшаблон — указать шаблон для поиска;
* -C — различать большие и малые буквы;
* -n — выдавать номера строк.

затем ищет в указанном файле нужные строки, определяемые ключом -p (Рис. 1.1-1.2).

![Рис. 1.1 (Командная строка 1)](image/1.jpg) 

Рис. 1.1 (Командная строка 1)

![Рис. 1.2 (Программа 1)](image/2.jpg) 

Рис. 1.2 (Программа 1)

2. Написал программу, которая вводит число и определяет, является ли оно больше нуля, меньше нуля или равно нулю (Рис. 2.1-2.2).

![Рис. 2.1 (Командная строка 2)](image/3.jpg) 

Рис. 2.1 (Командная строка 2)

![Рис. 2.2 (Программа 2)](image/4.jpg) 

Рис. 2.2 (Программа 2)

3. Написал командный файл, создающий указанное число файлов, пронумерованных последовательно от 1 до 𝑁 (например 1.tmp, 2.tmp, 3.tmp,4.tmp и т.д.). Число файлов, которые необходимо создать, передаётся в аргументы командной строки. Этот же командный файл умеет удалять все созданные им файлы (Рис. 3.1-3.2).

![Рис. 3.1 (Командная строка 3)](image/5.jpg) 

Рис. 3.1 (Командная строка 3)

![Рис. 3.2 (Программа 3)](image/6.jpg) 

Рис. 3.2 (Программа 3)

4. Написал командный файл, который с помощью команды tar запаковывает в архив все файлы в указанной директории. (Рис. 4.1-4.2)

![Рис. 4.1 (Командная строка 4)](image/7.jpg) 

Рис. 4.1 (Командная строка 4)

![Рис. 4.2 (Программа 4)](image/8.jpg) 

Рис. 4.2 (Программа 4)

## Вывод:

Я изучил основы программирования в оболочке ОС UNIX. Научился писать более сложные командные файлы с использованием логических управляющих конструкций и циклов.