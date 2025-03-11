---
## Front matter
title: "Отчет по лабораторной работе №5"
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

Получить основные навыки по настройке VLAN на коммутаторах сети.

# Задание

1. На коммутаторах сети настроить Trunk-порты на соответствующих интерфейсах, связывающих коммутаторы между
собой.

2. Коммутатор msk-donskaya-sw-1 настроить как VTP-сервер и прописать на нём номера и названия VLAN согласно табл. 3.1 из раздела 3.3.

3. Коммутаторы msk-donskaya-sw-2 — msk-donskaya-sw-4, mskpavlovskaya-sw-1 настроить как VTP-клиенты, на интерфейсах указать принадлежность к соответствующему VLAN.

4. На серверах прописать IP-адреса, как указано в табл. 3.2 из раздела 3.3.

5. На оконечных устройствах указать соответствующий адрес шлюза и прописать статические IP-адреса из диапазона соответствующей сети, следуя регламенту выделения ip-адресов.

6. Проверить доступность устройств, принадлежащих одному VLAN, и недоступность устройств, принадлежащих разным VLAN.

7. При выполнении работы необходимо учитывать соглашение об именовании.

# Выполнение лабораторной работы

1. Используя приведённую ниже последовательность команд, настроила Trunk-порты на соответствующих интерфейсах всех коммутаторов.

![*Настройка Trunk-портов на коммутаторе msk-donskaya-pilobanova-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/1.png){#fig:001 width=70%}

![*Настройка Trunk-портов на коммутаторе msk-donskaya-pilobanova-sw-2*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/2.png){#fig:002 width=70%}

![*Настройка Trunk-портов на коммутаторе msk-donskaya-pilobanova-sw-3*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/3.png){#fig:003 width=70%}

![*Настройка Trunk-портов на коммутаторе msk-donskaya-pilobanova-sw-4*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/4.png){#fig:004 width=70%}

![*Настройка Trunk-портов на коммутаторе msk-pavlovskaya-pilobanova-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/5.png){#fig:005 width=70%}

2. Используя приведённую ниже последовательность команд по конфигурации VTP, настроила коммутатор msk-donskaya-sw-1 как VTP-сервер и прописала на нём номера и названия VLAN.

![*Настройка коммутатора msk-donskaya-pilobanova-sw-1 как VTP-сервер*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/6.png){#fig:006 width=70%}

3. Используя приведённую ниже последовательность команд по конфигурации диапазонов портов, настроила коммутаторы msk-donskaya-sw-2 — mskdonskaya-sw-4, msk-pavlovskaya-sw-1 как VTP-клиенты и на интерфейсах указала принадлежность к VLAN.

![*Настройка коммутатора msk-donskaya-pilobanova-sw-2 как VTP-клиента*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/7.png){#fig:007 width=70%}

![*Настройка коммутатора msk-donskaya-pilobanova-sw-3 как VTP-клиента*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/8.png){#fig:008 width=70%}

![*Настройка коммутатора mskdonskaya-pilobanova-sw-4 как VTP-клиента*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/9.png){#fig:009 width=70%}

![*Настройка коммутатора msk-pavlovskaya-pilobanova-sw-1 как VTP-клиента*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/10.png){#fig:010 width=70%}

4. Указала статические IP-адреса на оконечных устройствах и серверах.

![*Указание шлюза для серверов*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/11.png){#fig:011 width=70%}

![*Указание IP-адреса для сервера web*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/12.png){#fig:012 width=70%}

![*Указание IP-адреса для сервера file*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/13.png){#fig:013 width=70%}

![*Указание IP-адреса для сервера mail*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/14.png){#fig:014 width=70%}

![*Указание шлюза для ДК (Донская)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/15.png){#fig:015 width=70%}

![*Указание IP-адреса для ДК (Донская)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/16.png){#fig:016 width=70%}

![*Указание шлюза для Кафедр*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/17.png){#fig:017 width=70%}

![*Указание IP-адреса для Кафедр*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/18.png){#fig:018 width=70%}

![*Указание шлюза для Администрации*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/19.png){#fig:019 width=70%}

![*Указание IP-адреса для Администрации*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/20.png){#fig:020 width=70%}

![*Указание шлюза для Других пользователей (Донская)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/21.png){#fig:021 width=70%}

![*Указание IP-адреса для Других пользователей (Донская)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/22.png){#fig:022 width=70%}

![*Указание шлюза для ДК (Павловская)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/23.png){#fig:023 width=70%}

![*Указание IP-адреса для ДК (Павловская)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/24.png){#fig:024 width=70%}

![*Указание шлюза для Других пользователей (Павловская)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/25.png){#fig:025 width=70%}

![*Указание IP-адреса для Других пользователей (Павловская)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/26.png){#fig:026 width=70%}

5. Проверила с помощью команды ping доступность устройств, принадлежащих одному VLAN (dk-donskaya-pilobanova-1 и dk-pavlovskaya-pilobanova-1), и недоступность устройств, принадлежащих разным VLAN (dk-donskaya-pilobanova-1 и other-pavlovskaya-pilobanova-1).

![*Команда ping*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/27.png){#fig:027 width=70%}

6. Используя режим симуляции в Packet Tracer, изучила процесс передвижения пакета ICMP по сети. Изучила содержимое передаваемого пакета и заголовки задействованных протоколов.

![*Движение пакета к dk-donskaya-pilobanova-1 от dk-pavlovskaya-pilobanova-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/28.png){#fig:028 width=70%}

![*Движение пакета к dk-donskaya-pilobanova-1 от other-pavlovskaya-pilobanova-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/29.png){#fig:029 width=70%}

![*Содержимое пакета ICMP*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/30.png){#fig:030 width=70%}

# Контрольные вопросы

1. Какая команда используется для просмотра списка VLAN на сетевом устройстве?

show vlan (sh vlan)

2. Охарактеризуйте VLAN Trunking Protocol (VTP). Приведите перечень команд с пояснениями для настройки и просмотра информации о VLAN.

Протокол VTP (англ. VLAN Trunking Protocol) — протокол ЛВС, служащий для обмена информацией о VLAN (виртуальных сетях), имеющихся на выбранном транковом порту. Разработан и используется компанией Cisco.

•	show vlan — выводит подробный список номеров и имён VLAN, активных на коммутаторе, а также портов, назначенных в каждую из них;

•	switchport access vlan vlan_number - команды для назначения отдельных портов в сети VLAN;

•	switchport access vlan vlan_number - команды для назначения диапазонов портов в сети VLAN.


3. Охарактеризуйте Internet Control Message Protocol (ICMP). Опишите формат пакета ICMP.

Протокол Internet Control Message Protocol (ICMP) – это набор коммуникационных правил, которые устройства используют для распространения информации об ошибках передачи данных в сети. При обмене сообщениями между отправителем и получателем могут возникнуть непредвиденные ошибки. Например, сообщения могут быть слишком длинными или пакеты данных могут приходить не по порядку, поэтому получатель не может их организовать.
Формат пакета ICMP включает следующие поля:

•	Идентификатор (обычно это идентификатор процесса) и номер по порядку (увеличивается на 1 при посылке каждого пакета). Эти поля служат для того, чтобы отправитель мог связать в пары запросы и отклики.

•	Тип определяет, является ли этот пакет запросом (8) или откликом (0).

•	Контрольная сумма представляет собой 16-разрядное дополнение по модулю 1 контрольной суммы всего ICMP-сообщения, начиная с поля тип.

•	Данные служит для записи информации, возвращаемой отправителю.

4. Охарактеризуйте Address Resolution Protocol (ARP). Опишите формат пакета ARP.

ARP - протокол разрешения адресов (Address Resolution Protocol) является протоколом третьего (сетевого) уровня модели OSI, используется для преобразования IP-адресов в MAC-адреса, играет важную функцию в множественном доступе сетей.
Формат сообщения ARP включает следующие поля:

•	Тип оборудования. Размер поля равен 2 байтам. Определяет тип оборудования, используемое для передачи сообщения. Наиболее распространённый тип оборудования — Ethernet. Значение Ethernet равно 1.

•	Тип протокола. Указывает, какой протокол использовался для передачи сообщения. Значение этого поля равно 2048, что указывает на IPv4.

•	Длина аппаратного адреса. Показывает длину сетевого адреса в байтах. Размер MAC-адреса Ethernet составляет 6 байт.

•	Длина адреса протокола. Показывает размер IP-адреса в байтах. Размер IP-адреса равен 4 байтам.

•	Операционный закон. Указывает тип сообщения. Если значение этого поля равно 1, то это сообщение-запрос, а если значение этого поля равно 2, то это ответное сообщение.

•	Аппаратный адрес отправителя. Содержит MAC-адрес устройства, передающего сообщение.

5. Что такое MAC-адрес? Какова его структура?

MAC-адрес — это уникальный код, присвоенный производителем сетевому устройству (например, беспроводному сетевому адаптеру или ethernet-адаптеру). MAC — это сокращение от Media Access Control. Предполагается, что каждый код является уникальным для определённого устройства. MAC-адрес состоит из шести групп по два символа, разделённых двоеточиями.

# Выводы

Я получила основные навыки по настройке VLAN на коммутаторах сети.

# Список литературы{.unnumbered}

::: {#refs}
:::
