---
## Front matter
title: "Отчет по лабораторной работе №4"
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

Провести подготовительную работу по первоначальной настройке коммутаторов сети.

# Задание

Требуется сделать первоначальную настройку коммутаторов сети, представленной на схеме L1 (см. рис. 3.1 из раздела 3.3). Под первоначальной настройкой понимается указание имени устройства, его IP-адреса, настройка доступа по паролю к виртуальным терминалам и консоли, настройка удалённого доступа к устройству по ssh. При выполнении работы необходимо учитывать соглашение об именовании.


# Выполнение лабораторной работы

1. В логической рабочей области Packet Tracer разместила коммутаторы и оконечные устройства согласно схеме сети L1 и соединила их через соответствующие интерфейсы.

![*Схема сети L1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab4/report/image/1.png){#fig:001 width=70%}

2. Используя типовую конфигурацию коммутатора, настроила все коммутаторы, изменяя название устройства и его IP-адрес согласно плану IP.

![*Настройка коммутатора msk-donskaya-pilobanova-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab4/report/image/2.png){#fig:002 width=70%}

![*Настройка коммутатора msk-donskaya-pilobanova-sw-2*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab4/report/image/3.png){#fig:003 width=70%}

![*Настройка коммутатора msk-donskaya-pilobanova-sw-3*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab4/report/image/4.png){#fig:004 width=70%}

![*Настройка коммутатора msk-donskaya-pilobanova-sw-4*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab4/report/image/5.png){#fig:005 width=70%}

![*Настройка коммутатора msk-pavlovskaya-pilobanova-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab4/report/image/6.png){#fig:006 width=70%}


# Выводы

Я провела подготовительную работу по первоначальной настройке коммутаторов сети.

# Контрольные вопросы

1. При помощи каких команд можно посмотреть конфигурацию сетевого оборудования?

show running-config

sh ru

2. При помощи каких команд можно посмотреть стартовый конфигурационный файл оборудования?

show startup-config

3. При помощи каких команд можно экспортировать конфигурационный файл оборудования?

При помощи кнопки export в окне для конфигурации устройства

4. При помощи каких команд можно импортировать конфигурационный файл оборудования?

При помощи кнопки import в окне для конфигурации устройства

# Список литературы{.unnumbered}

::: {#refs}
:::

