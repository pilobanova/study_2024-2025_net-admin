---
## Front matter
title: "Отчет по лабораторной работе №16"
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

Получение навыков настройки VPN-туннеля через незащищённое Интернет-соединение.

# Задание

Настроить VPN-туннель между сетью Университета г. Пиза (Италия) и сетью «Донская» в г. Москва.
При выполнении работы необходимо учитывать соглашение об именовании.

# Выполнение лабораторной работы

1. Разместила в рабочей области проекта в соответствии с модельными предположениями оборудование для сети Университета г. Пиза.

![*Медиаконвертер с модулями PT-REPEATERNM-1FFE и PT-REPEATER-NM-1CFE*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab16/report/image/1.png){#fig:001 width=70%}

![*Схема сети с дополнительными площадками*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab16/report/image/2.png){#fig:002 width=70%}

2. В физической рабочей области проекта создала город Пиза, здание Университета г. Пиза. Переместила туда соответствующее оборудование.

![*Здание в г. Пиза*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab16/report/image/3.png){#fig:003 width=70%}

3. Сделать первоначальную настройку и настройку интерфейсов оборудования сети Университета г. Пиза.

![*Первоначальная настройка маршрутизатора pisa-unipi-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab16/report/image/4.png){#fig:004 width=70%}

![*Первоначальная настройка коммутатора pisa-unipi-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab16/report/image/5.png){#fig:005 width=70%}

![*Настройка интерфейсов маршрутизатора pisa-unipi-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab16/report/image/6.png){#fig:006 width=70%}

![*Настройка интерфейсов коммутатора pisa-unipi-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab16/report/image/7.png){#fig:007 width=70%}

4. Настроила VPN на основе протокола GRE.

![*Настройка маршрутизатора msk-donskaya-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab16/report/image/8.png){#fig:008 width=70%}

![*Настройка маршрутизатора pisa-unipi-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab16/report/image/9.png){#fig:009 width=70%}


# Выводы

Я получила навыки настройки VPN-туннеля через незащищённое Интернет-соединение.

# Контрольные вопросы

1. Что такое VPN?

Виртуальная частная сеть (Виртуальная частная сеть, VPN) — технология, обеспечивающая одно или несколько сетевых соединений через другую сеть (например, Интернет).

2. В каких случаях следует использовать VPN?

VPN шифрует интернет-трафик, защищая данные от хакеров и интернет-провайдеров, что особенно важно в общедоступных Wi-Fi-сетях. Он скрывает реальный IP-адрес, предотвращая отслеживание местонахождения и онлайн-активности. VPN помогает обойти цензуру и географические ограничения, обеспечивая доступ к заблокированным сайтам и внешнему контенту. Это также незаменимо для безопасной работы в корпоративных сетях, позволяя сотрудникам удаленно подключаться к корпоративным ресурсам и защищать корпоративные данные от несанкционированного доступа. VPN защищает от атак типа «человек посередине» и блокирует конкурентные веб-сайты и фишинговые атаки. Это также позволяет экономить на покупках, предоставляя доступ к региональным ценам на товары и услуги в Интернете. Примеры использования VPN включают защиту личной информации в общедоступных сетях Wi-Fi, обход внешних ограничений, безопасную удаленную работу и анонимный серфинг. В современном цифровом мире, где угрозы кибербезопасности и ограничения доступа становятся все более распространенными, VPN является мощным средством обеспечения безопасности и конфиденциальности.

3. Как с помощью VPN обойти NAT?

Обход NAT с помощью VPN возможен благодаря тому, что VPN обеспечивает зашифрованное соединение между телефонным пользователем и удаленным сервером, минуя при этом ограничения, налагаемые NAT. Это позволяет устройству пользователя получать данные через Интернет, исключая ограничения NAT.

# Список литературы{.unnumbered}

::: {#refs}
:::
