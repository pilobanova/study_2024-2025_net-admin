---
## Front matter
title: "Отчет по лабораторной работе №13"
subtitle: "Дисциплина: Администрирование локальных сетей"
author: "Лобанова Полина Иннокентьевна"

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

Провести подготовительные мероприятия по организации взаимодействия через сеть провайдера посредством статической маршрутизации локальной сети с сетью основного здания, расположенного в 42-м квартале в Москве, и сетью филиала, расположенного в г. Сочи.

# Задание

1. Внести изменения в схемы L1, L2 и L3 сети, добавив в них информацию о сети основной территории (42-й квартал в Москве) и сети филиала в г. Сочи.

2. Дополнить схему проекта, добавив подсеть основной территории организации 42-го квартала в Москве и подсеть филиала в г. Сочи.

3. Сделать первоначальную настройку добавленного в проект оборудования.

4. При выполнении работы необходимо учитывать соглашение об именовании.

# Выполнение лабораторной работы

1. Внесла изменения в схемы L1, L2 и L3 сети.

![*Схема L1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab13/report/image/1.png){#fig:001 width=70%}

![*Схема L2*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab13/report/image/2.png){#fig:002 width=70%}

![*Схема L3*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab13/report/image/3.png){#fig:003 width=70%}

2. На схеме предыдущего проекта разместила необходимое оборудование: 4 медиаконвертера (Repeater-PT), 2 маршрутизатора типа Cisco 2811, 1 маршрутизирующий коммутатор типа Cisco 3560-24PS, 2 коммутатора типа Cisco 2950-24, коммутатор Cisco 2950-24T, 3 оконечных устройства типа PC-PT и присвоила названия размещённым объектам.

![*Схема сети с дополнительными площадками*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab13/report/image/4.png){#fig:004 width=70%}

3. На медиаконвертерах заменила имеющиеся модули на PT-REPEATERNM-1FFE и PT-REPEATER-NM-1CFE для подключения витой пары по технологии Fast Ethernet и оптоволокна соответственно.

![*Медиаконвертер с модулями PT-REPEATER-NM-1FFE и PT-REPEATER-NM-1CFE*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab13/report/image/5.png){#fig:005 width=70%}

4. На маршрутизаторе msk-q42-gw-1 добавила дополнительный интерфейс NM-2FE2W.

![*Маршрутизатор с дополнительным интерфейсом NM-2FE2W*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab13/report/image/6.png){#fig:006 width=70%}

5. В физической рабочей области Packet Tracer добавила в г. Москва здание 42-го квартала и присвоила ему соответствующее название.

![*Здание основной территории организации в Москве на физической схеме проекта*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab13/report/image/7.png){#fig:007 width=70%}

6. В физической рабочей области Packet Tracer добавила город Сочи и в нём здание филиала, присвоила ему соответствующее название.

![*Москва и Сочи на физической схеме проекта*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab13/report/image/8.png){#fig:008 width=70%}

7. Перенесила из сети «Донская» оборудование сети 42-го квартала и сети филиала в соответствующие здания.

![*Размещение объектов в основном здании 42-го квартала в Москве*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab13/report/image/10.png){#fig:009 width=70%}

![*Размещение объектов в здании филиала в г.Сочи*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab13/report/image/9.png){#fig:010 width=70%}

8. Сделала первоначальную настройку добавленного в проект оборудования.

![*Первоначальная настройка маршрутизатора msk-q42-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab13/report/image/11.png){#fig:011 width=70%}

![*Первоначальная настройка коммутатора msk-q42-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab13/report/image/12.png){#fig:012 width=70%}

![*Первоначальная настройка маршрутизирующего коммутатора msk-hostel-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab13/report/image/13.png){#fig:013 width=70%}

![*Первоначальная настройка коммутатора msk-hostel-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab13/report/image/14.png){#fig:014 width=70%}

![*Первоначальная настройка коммутатора sch-sochi-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab13/report/image/15.png){#fig:015 width=70%}

![*Первоначальная настройка маршрутизатора sch-sochi-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab13/report/image/16.png){#fig:016 width=70%}



# Выводы

Я провела подготовительные мероприятия по организации взаимодействия через сеть провайдера посредством статической маршрутизации локальной сети с сетью основного здания, расположенного в 42-м квартале в Москве, и сетью филиала, расположенного в г. Сочи.

# Список литературы{.unnumbered}

::: {#refs}
:::
