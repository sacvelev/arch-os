---
## Front matter
title: "Индивидуальный проект. Персональный сайт научного работника"
subtitle: "Этап 1"
author: "Цвелев С.А. НПИбд-02-22"

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
  
  Быстрое развертывание сайта на GitHub Pages с помощью генератора статического html Hugo.

# Выполнение проекта

1. Устанавливаем программное обеспечение hugo.

![Установка hugo через терминал](image/01.png){ #fig:001 width=70%, height=70% }

2. Создаем репозиторий blog, используя шаблон. После, используя hugo, компилируем сервер.

![Компиляция через hugo](image/02.png){ #fig:001 width=70%, height=70% }

3. Для публикации сайта нужно создать отдельный репозиторий.

![Создание репозитория - <имяпользователя>.github.io](image/03.png){ #fig:001 width=70%, height=70% }

4. С помощью команды git submodule добавляем репозиторий из public в индекс, предварительно убрав public из .gitignore. Используем команду hugo, а затем с помощью git push заливаем файлы в репозиторий. Сайт создан.

![Использование команды git submodule](image/04.png){ #fig:001 width=70%, height=70% }

![Готовый сайт](image/05.png){ #fig:001 width=70%, height=70% }

# Вывод

Мы смогли сделать заготовку для сайта на Github с помощью hugo.