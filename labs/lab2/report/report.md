---
## Front matter
title: "Отчет по лабораторной работе №2"
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

Получить основные навыки по начальному конфигурированию оборудования Cisco.

# Задание

1. Сделать предварительную настройку маршрутизатора:

– задать имя в виде «город-территория-учётная_записьтип_оборудования-номер»;

– задать интерфейсу Fast Ethernet с номером 0 ip-адрес 192.168.1.254 и маску 255.255.255.0, затем поднять интерфейс;

– задать пароль для доступа к привилегированному режиму (сначала в открытом виде, затем — в зашифрованном);

– настроить доступ к оборудованию сначала через telnet, затем — через ssh;

– сохранить и экспортировать конфигурацию в отдельный файл.

2. Сделать предварительную настройку коммутатора:

– задать имя в виде «город-территория-учётная_записьтип_оборудования-номер»;

– задать интерфейсу vlan 2 ip-адрес 192.168.2.1 и маску 255.255.255.0, затем поднять интерфейс;

– привязать интерфейс Fast Ethernet с номером 1 к vlan 2;

– задать в качестве адреса шлюза по умолчанию адрес 192.168.2.254;

– задать пароль для доступа к привилегированному режиму (сначала в открытом виде, затем — в зашифрованном);

– настроить доступ к оборудованию сначала через telnet, затем — через ssh;

– для пользователя admin задать доступ 1-го уровня по паролю;

– сохранить и экспортировать конфигурацию в отдельный файл.


# Выполнение лабораторной работы

1. В логической рабочей области Packet Tracer разместила коммутатор, маршрутизатор и 2 оконечных устройства типа PC, соединила один PC с маршрутизатором, другой PC — с коммутатором.

![*Топология*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/1.png){#fig:001 width=70%}

2. Провела настройку маршрутизатора. Задала имя в виде «город-территория-учётная_записьтип_оборудования-номер».

![*Имя маршрутизатора*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/2.png){#fig:002 width=70%}

3. Задала интерфейсу Fast Ethernet с номером 0 ip-адрес 192.168.1.254 и маску 255.255.255.0, затем подняла интерфейс.

![*Назначение ip-адреса*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/3.png){#fig:003 width=70%}

4. Проверила работоспособность соединений с помощью команды ping.

![*ip-адрес PC*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/4.png){#fig:004 width=70%}

![*Команда ping*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/5.png){#fig:005 width=70%}

5. Задала пароль для доступа к привилегированному режиму (сначала в открытом виде, затем — в зашифрованном).

![*Установка пароля*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/6.png){#fig:006 width=70%}

![*Установка пароля*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/8.png){#fig:007 width=70%}

![*Установка пароля*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/9.png){#fig:008 width=70%}

5. Настроила доступ к оборудованию через telnet.

![*Подключение через telnet*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/7.png){#fig:009 width=70%}

![*Подключение через telnet*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/10.png){#fig:010 width=70%}

6. Для пользователя admin задала доступ 1-го уровня по паролю.

![*Установка пароля для пользователя*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/11.png){#fig:011 width=70%}

7. Настроила доступ к оборудованию через ssh.

![*Создания пароля*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/12.png){#fig:012 width=70%}

![*Подключение через ssh*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/13.png){#fig:013 width=70%}

8. Сохранила и экспортировала конфигурацию в отдельный файл.

9. Провела настройку коммутатора. Задала имя в виде «город-территория-учётная_записьтип_оборудования-номер».

![*Имя коммутатора*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/14.png){#fig:014 width=70%}

10. Задала интерфейсу vlan 2 ip-адрес 192.168.2.1 и маску 255.255.255.0, затем подняла интерфейс.

![*Назначение ip-адреса*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/15.png){#fig:015 width=70%}

11. Привязала интерфейс Fast Ethernet с номером 1 к vlan 2.

![*Привязка интерфейса Fast Ethernet к vlan 2*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/16.png){#fig:016 width=70%}

12. Задала в качестве адреса шлюза по умолчанию адрес 192.168.2.254.

![*Назначение адреса шлюза*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/17.png){#fig:017 width=70%}

13. Проверила работоспособность соединений с помощью команды ping.

![*Команда ping*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/18.png){#fig:018 width=70%}

14. Задала пароль для доступа к привилегированному режиму (сначала в открытом виде, затем — в зашифрованном).

![*Установка пароля*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/19.png){#fig:019 width=70%}

![*Установка пароля*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/20.png){#fig:020 width=70%}

![*Установка пароля*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/21.png){#fig:021 width=70%}

15. Настроила доступ к оборудованию через telnet.

![*Подключение через telnet*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/22.png){#fig:022 width=70%}

16. Для пользователя admin задала доступ 1-го уровня по паролю.

![*Установка пароля для пользователя*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/23.png){#fig:023 width=70%}

17. Настроила доступ к оборудованию через ssh.

![*Создания пароля*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/24.png){#fig:024 width=70%}

![*Подключение через ssh*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/25.png){#fig:025 width=70%}

18. Сохранила и экспортировала конфигурацию в отдельный файл.



# Выводы

Получить получила основные навыки по начальному конфигурированию оборудования Cisco.


