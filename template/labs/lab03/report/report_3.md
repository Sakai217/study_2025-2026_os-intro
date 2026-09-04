---
mainfont: LiberationSerif
sansfont: LiberationSans
monofont: LiberationMono
geometry: margin=2cm
pdf-engine: xelatex

## Front matter
title: "Лабораторная работа №3"
subtitle: "Markdown"
author: "Гаджимурадов Аяз Тахирович"

## Generic options
lang: ru-RU\
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true
toc-depth: 2
lof: true
lot: true
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt

---
# Цель работы

Научиться оформлять отчеты с помощью легковесного языка разметки Markdown.

# Задание

- Сделать отчёт по предыдущей лабораторной работе в формате Markdown.
- В качестве отчёта предоставить отчёты в 3 форматах: pdf, docx и md (в архиве,
поскольку он должен содержать скриншоты, Makefile и т.д.)

# Теоретические введение

Markdown - это легкий язык разметки для оформления текста. 

Он нужен, чтобы писать читаемый текст в обычном блокноте, который автоматически превращается в красиво отформатированный на GitHub.

# Выполнение лабораторной работы

Перехожу в директорию в которой рапологается шаблон для отчета по лабораторной работе.
Открываю файл шаблона с помощью текстового редактора и начинаю заполнять его.

![](image/2.png){width=70%}

После изменения шаблона я переименовываю его и выполняю компиляцию в форматы docx и pdf из формата md.

![](image/3.png){width=70%}

Далее отправляю созданные файлы на глобальный репозиторий.

![](image/4.png){width=70%}

Завершаю отправку с помощью git push.

![](image/5.png){width=70%}

# Вывод

В ходе работы были изучены базовые элементы Markdown.

