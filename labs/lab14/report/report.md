---
## Front matter
title: "Отчет по лабораторной работе № 14"
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

Настроить взаимодействие через сеть провайдера посредством статической маршрутизации локальной сети организации с сетью основного здания, расположенного в 42-м квартале в Москве, и сетью филиала, расположенного в г. Сочи.

# Задание

1. Настроить связь между территориями.

2. Настроить оборудование, расположенное в квартале 42 в Москве.

3. Настроить оборудование, расположенное в филиале в г. Сочи.

4. Настроить статическую маршрутизацию между территориями.

5. Настроить статическую маршрутизацию на территории квартала 42 в г. Москве.

6. Настроить NAT на маршрутизаторе msk-donskaya-gw-1.

7. При выполнении работы необходимо учитывать соглашение об именовании.


# Выполнение лабораторной работы

1. Настроила связь между территориями.

![*Настройка интерфейсов коммутатора provider-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/1.png){#fig:001 width=70%}

![*Настройка интерфейсов маршрутизатора msk-donskaya-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/2.png){#fig:002 width=70%}

![*Настройка интерфейсов маршрутизатора msk-q42-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/3.png){#fig:003 width=70%}

![*Настройка интерфейсов коммутатора sch-sochi-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/4.png){#fig:004 width=70%}

![*Настройка интерфейсов маршрутизатора sch-sochi-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/5.png){#fig:005 width=70%}

2. Настроила оборудование, расположенное в квартале 42 в Москве.

![*Настройка интерфейсов маршрутизатора msk-q42-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/6.png){#fig:006 width=70%}

![*Настройка интерфейсов коммутатора msk-q42-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/7.png){#fig:007 width=70%}

![*Настройка интерфейсов маршрутизирующего коммутатора msk-hostel-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/8.png){#fig:008 width=70%}

![*Настройка интерфейсов коммутатора msk-hostel-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/9.png){#fig:009 width=70%}

3. Настроила оборудование, расположенное в филиале в г. Сочи.

![*Настройка интерфейсов маршрутизатора sch-sochi-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/10.png){#fig:010 width=70%}

![*Настройка интерфейсов коммутатора sch-sochi-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/11.png){#fig:011 width=70%}

4. Настроила статическую маршрутизацию между территориями.

![*Настройка маршрутизатора msk-donskaya-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/12.png){#fig:012 width=70%}

![*Настройка маршрутизатора msk-q42-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/13.png){#fig:013 width=70%}

![*Настройка маршрутизатора sch-sochi-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/14.png){#fig:014 width=70%}

5. Настроила статическую маршрутизацию на территории квартала 42 в г. Москве.

![*Настройка маршрутизатора msk-q42-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/15.png){#fig:015 width=70%}

![*Настройка интерфейсов маршрутизирующего коммутатора msk-hostel-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/16.png){#fig:016 width=70%}

6. Настроила NAT на маршрутизаторе msk-donskaya-gw-1.

![*Настройка NAT на маршрутизаторе msk-donskaya-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/17.png){#fig:017 width=70%}


# Выводы

Я настроила взаимодействие через сеть провайдера посредством статической маршрутизации локальной сети организации с сетью основного здания, расположенного в 42-м квартале в Москве, и сетью филиала, расположенного в г. Сочи.

# Контрольные вопросы

1. Приведите пример настройки статической маршрутизации между двумя подсетями организации.

(config)# ip route 192.168.2.0 255.255.255.0 192.168.1.2

(config)# ip route 192.168.1.0 255.255.255.0 192.168.2.1

2. Опишите процесс обращения устройства из одного VLAN к устройству из другого VLAN.

Определение VLAN:
Устройства в повышении мощности сети различных VLAN для управления трафиком и безопасности. Каждая VLAN представляет собой логическую сеть сегментации, при которой устройство может общаться только в пределах своей VLAN.

Маршрутизация между VLAN:
Для обращения устройства из одной VLAN к устройству из другой VLAN требуется маршрутизация между VLAN. Этого можно добиться с помощью маршрутизатора или многоуровневого коммутатора, способного работать на уровне маршрутизации.

Пересылка трафика:
Когда устройство из одной VLAN отправляет пакет устройству из другой VLAN, маршрутизатор или многоуровневый коммутатор принимает пакет, затем его адрес и пересылает его в соответствующую VLAN.

Priem traffic:
Устройство в целевом VLAN принимает пакет и обрабатывает его в соответствии с его адресом и стандартом безопасности VLAN.

3. Как проверить работоспособность маршрута?

Командой ping или traceroute.

4. Как посмотреть таблицу маршрутизации?

Командой show ip route


# Список литературы{.unnumbered}

::: {#refs}
:::
