---
## Front matter
title: "Отчет по лабораторной работе №11"
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

Провести подготовительные мероприятия по подключению локальной сети организации к Интернету.

# Задание

1. Построить схему подсоединения локальной сети к Интернету.

2. Построить модельные сети провайдера и сети Интернет.

3. Построить схемы сетей L1, L2, L3.

4. При выполнении работы необходимо учитывать соглашение об именовании.

![](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab11/report/image/1.png){#fig:000 width=70%}

Модельные предположения:

– В сети провайдера располагаются 2 медиаконвертера provider-mc-1 и provider-mc-2 для связи с подсетью «Донская» и сетью модельного Интернета, маршрутизатор provider-gw-1 и коммутатор provider-sw-1. Оборудование соединяется между собой по Fast Ethernet согласно схеме.

– В модельной сети Интернет располагаются 4 сервера www.yandex.ru, www.rudn.ru, stud.rudn.university и esystem.pfur.ru, коммутатор internet-sw-1 и медиаконвертер internet-mc-1 для связи с сетью провайдера. Серверы подключены к коммутатору посредством Fast Ethernet, коммутатор подсоединён к медиаконвертеру также по Fast Ethernet.

– Имена и адреса серверам Интернета и маршрутизатору провайдера задаются согласно табл. 11.1. При этом учитывается, что под сеть адресов модельного Интернета выделяется адрес 192.0.2.0/24, а под сеть провайдера — 198.51.100.1.

# Выполнение лабораторной работы

1. Внесла изменения в схему L1 сети, добавив в неё сеть провайдера и сеть модельного Интернета с указанием названий оборудования и портов подключения.

![*Физические устройства сети с номерами портов (Layer 1)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab11/report/image/2.png){#fig:001 width=70%}

2. Внесла изменения в схемы L2 и L3 сети, указав адреса и VLAN сети провайдера и модельной сети Интернета. Скорректировала таблицы распределения IP-адресов и портов.

![*Схема VLAN сети (Layer 2)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab11/report/image/3.png){#fig:002 width=70%}

![*Схема маршрутизации сети (Layer 3)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab11/report/image/4.png){#fig:003 width=70%}

![*Таблица IP*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab11/report/image/5.png){#fig:004 width=70%}

![*Таблица портов*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab11/report/image/6.png){#fig:005 width=70%}

3. На схеме предыдущего проекта разместила согласно рис. 11.2 необходимое оборудование для сети провайдера и сети модельного Интернета: 4 медиаконвертера (Repeater-PT), 2 коммутатора типа Cisco 2960-24TT, маршрутизатор типа Cisco 2811, 4 сервера. Присвоила названия размещённым в сети провайдера и в сети модельного Интернета объектам согласно модельным предположениям и схеме L1.

![*Схема сети с выходом в Интернет*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab11/report/image/7.png){#fig:006 width=70%}

4. В физической рабочей области добавила здание провайдера и здание, имитирующее расположение серверов модельного Интернета. Присвоила им соответствующие названия.

![*Схема сети в физической рабочей области Packet Tracer*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab11/report/image/8.png){#fig:007 width=70%}

5. Перенесла из сети «Донская» оборудование провайдера и модельной сети Интернета в соответствующие здания.

![*Оборудование в здании сети провайдера*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab11/report/image/9.png){#fig:008 width=70%}

![*Оборудование в здании сети модельного Интернета*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab11/report/image/10.png){#fig:009 width=70%}

6. На медиаконвертерах заменила имеющиеся модули на PT-REPEATERNM-1FFE и PT-REPEATER NM-1CFE для подключения витой пары по технологии Fast Ethernet и оптоволокна соответственно.

![*Медиаконвертер с модулями PT-REPEATER-NM-1FFE и PT-REPEATER-NM-1CFE*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab11/report/image/11.png){#fig:010 width=70%}

7. Провела соединение объектов согласно скорректированной схеме L1.

![*Схема сети с выходом в Интернет*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab11/report/image/12.png){#fig:011 width=70%}

8. Прописала IP-адреса серверам согласно табл. 11.1.

![*Назначение адреса шлюза*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab11/report/image/13.png){#fig:012 width=70%}

![*Назначение IP-адреса*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab11/report/image/14.png){#fig:013 width=70%}

9. Прописала сведения о серверах на DNS-сервере сети «Донская».

![*DNS-записи на сервере DNS в сети «Донская»*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab11/report/image/15.png){#fig:014 width=70%}


# Выводы

Я провела подготовительные мероприятия по подключению локальной сети организации к Интернету.

# Контрольные вопросы

1. Что такое трансляция сетевых адресов (NAT)?

Network Address Translation (NAT) — механизм преобразования IP-адресов транзитных пакетов. В частности, механизм NAT используется для обеспечения доступа устройств к локальным сетям с защитой IP-адресов сети от сети Интернет.

2. Как определить, находится ли узел сети за NAT?

Проанализируйте прерывание конфигурации маршрутизатора или другого сетевого оборудования, которое может выполнять функцию NAT.

3. Какое оборудование отвечает за преобразование адресов методом NAT?

Преобразование адреса методом NAT может создавать почти любой маршрутизирующий маршрутизатор — маршрутизатор, серверный доступ, межсетевой экран. Наиболее распространенным является SNAT, основной механизм, который состоит из замены источника адреса (англ. source) при построении пакета в одну сторону и обратной замены адресата (англ. Destination) в ответном пакете.

4. В чем отличие статического, динамического и перегруженного NAT?

Статические углы преобразования адресов по принципу 1:1, движущий 1:N, а перегруженный N:1.

5. Охарактеризуйте типы NAT.

Типы NAT:

1) статический NAT (Static NAT, SNAT) -- преобразование адресов по принципу 1:1 (в частности, один локальный IP-адрес преобразуется во внешний адрес, выделенный, например, провайдером);

2) активный NAT (Dynamic NAT, DNAT) -- преобразование адресов влево по принципу 1:N (например, один адрес устройства в локальной сети преобразуется в один из адресов внешних адресов);

3) Перегрузка NAT (или NAT Masquerading, или Port Address Translation, PAT) -- преобразование адресов влево по принципу N:1 (например, адреса группы устройств локальной подсети преобразуются в один внешний адрес, при этом дополнительно используется механизм адресации через номера портов).

# Список литературы{.unnumbered}

::: {#refs}
:::
