---
## Front matter
lang: ru-RU
title: "Лабораторная работа №3: отчет."
subtitle: "Markdown."
author: "Евдокимов Максим Михайлович. Группа - НФИбд-01-20."

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

Научиться оформлять отчёты с помощью легковесного языка разметки Markdown.

# Задание

1. Сделайте отчёт по предыдущей лабораторной работе в формате Markdown.
2. В качестве отчёта просьба предоставить отчёты в 3 форматах: pdf, docx и md (в архиве, поскольку он должен содержать скриншоты, Makefile и т.д.)

# Указание к работе

## Описание метода

- Заголовки (огловление) в markdown строются максимально просто:

``` markdown
# Основной заголовок (1 уровень)
## Подзаголовок (2 уровень)
### Раздел (3 уровень)
#### Подраздел (4 уровень)
```

- Также для работы с текстом есть простые способы отображения как в word:

``` markdown
*Жирный текст*
**Курсивный текст**
***Полужирный (курсивный) текст***
```

- Для работы со списками и цитатами есть данные структуры:

``` markdown
> цитата
  и её продолжение

- не 
- пронумерованный 
- список

1. пронумерованный
2. список
3. данных

1. многоуровневый
    1. список
      - разного 
      - типа
```

Для любых гиперссылок и файлов у нас есть данные структуры:

``` markdown
(название)[ссылка]
```

А для работы с разным типом кодов можно использоватьподобнуж структуру:

``` markdown
    ``` python
    print("Hello World!")
    ```
```

И для разного вида формул можно использовать несколько встренные структур или latex:

``` markdown

2^10^

$$\left( \sum_{k=1}^n a_k b_k \right)^2 \leq \left( \sum_{k=1}^n a_k^2 \right) \left( \sum_{k=1}^n b_k^2 \right)$$

```

И многие другие которые более специфичные.

# Выполнение лабораторной работы

Основные задачи данной лабораторной раюоты были выполнены в рамках предыдущих лабораторных.

# Выводы

В ходе выполнения данной лабораторной работы были повторены основные методы и принципы работы с markdown и pandoc.

# Список литературы {.unnumbered}

1. [Лабораторная работа №3](https://esystem.rudn.ru/mod/resource/view.php?id=970821)
2. [Онлайн редактор markdown](https://dillinger.io)
3. [Удобный сайт для построение latex структур](https://latexeditor.lagrida.com)
4. [Базовый синтаксис markdown для github](https://docs.github.com/ru/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
5. [Построение формул в markdown](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
