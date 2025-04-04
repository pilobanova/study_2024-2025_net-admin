---
## Front matter
lang: ru-RU
title: "Презентация по лабораторной работе №3"
subtitle: "Дисциплина: Администрирование локальных сетей"
author:
  - Лобанова П.И.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 28 февраля 2025

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---

# Информация

## Докладчик


  * Лобанова Полина Иннокентьевна
  * Учащаяся на направлении "Фундаментальная информатика и информационные технологии"
  * Студентка группы НФИбд-02-22
  * [polla-2004@mail.ru](polla-2004@mail.ru)
  

# Цель

Познакомится с принципами планирования локальной сети организации.

# Задание

Предположим, что в некоторой учебной организации требуется спланировать
сетевую инфраструктуру.
Особенности организации с точки зрения планирования локальной сети:

– организация располагается в одном городе (предположим — в Москве), но на двух территориях (назовём их «Донская» и «Павловская»);

– группы пользователей организации:

– администрация (А);

– преподавательский состав кафедр (К);

– пользователи дисплейных классов общего пользования (ДК);

– другие пользователи (Д);

##

– предполагается, что на территории «Донская» будут располагаться:

– устройства управления сетью;

– серверная инфраструктура;

– оборудование всех групп пользователей;

– предполагается, что на территории «Павловская» будет располагаться оборудование групп пользователей «ДК» и «Д».

##

Сеть организации должна соответствовать так называемой «иерархической модели сети», т.е. оборудование сетевой инфраструктуры при планировании должно быть распределено по трём уровням:

1) уровень ядра (Core Layer) — высокопроизводительные сетевые устройства (коммутаторы, маршрутизаторы), обеспечивающие скоростную передачу трафика между сегментами уровня распределения;

2) уровень распределения (Distribution Layer) — устройства (коммутаторы, маршрутизаторы), обеспечивающие применение политик безопасности и качества обслуживания (QoS), агрегацию и маршрутизацию трафика посредством VLAN, определение широковещательных доменов;

3) уровень доступа (Access Layer) — устройства для подключения серверов и оконечного оборудования пользователей к сети организации.

##

Далее при проектировании сети необходимо:

– разработать схемы сети, соответствующие физическому, канальному и сетевому уровням эталонной модели взаимодействия открытых систем (OSI);

– составить план IP-адресация сети;

– составить план VLAN сети;

– составить план подключения интерфейсов оборудования;

– зафиксировать перечень устройств, используемых в сети организации, с указанием модели, версии операционной системы, объёма RAM/NVRAM, списка интерфейсов;

– обеспечить маркировку всех задействованных как сетевых и других типов кабелей (откуда и куда идёт), так и устройств сети;

– разработать и внедрить единый регламент эксплуатации сети.

##

Задание:

1. Используя графический редактор (например, Dia), требуется повторить схемы L1, L2, L3, а также сопутствующие им таблицы VLAN, IP-адресов и портов подключения оборудования планируемой сети.

2. Рассмотренный выше пример планирования адресного пространства сети базируется на разбиении сети 10.128.0.0/16 на соответствующие подсети. Требуется сделать аналогичный план адресного пространства для сетей 172.16.0.0/12 и 192.168.0.0/16 с соответствующими схемами сети и сопутствующими таблицами VLAN, IP-адресов и портов подключения оборудования.

# Выполнение

Используя графический редактор Dia, повторила схемы L1, L2, L3.

![*Физические устройства сети с номерами портов (Layer 1)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab3/report/image/3.png){#fig:001 width=70%}

## 

![*Схема VLAN сети (Layer 2)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab3/report/image/1.png){#fig:002 width=70%}


## 

![*Схема маршрутизации сети (Layer 3)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab3/report/image/4.png){#fig:003 width=70%}

## 

Также повторила таблицы VLAN, IP-адресов и портов подключения оборудования планируемой сети.

![*Таблица VLAN*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab3/report/image/2.png){#fig:004 width=70%}

## 

![*Таблица IP*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab3/report/image/5.png){#fig:005 width=70%}

## 

![*Таблица портов*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab3/report/image/6.png){#fig:006 width=70%}

## 

![*Регламент выделения ip-адресов (для сети класса C)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab3/report/image/7.png){#fig:007 width=70%}

## 

Сделала аналогичный план адресного пространства для сети 172.16.0.0/12 с соответствующими схемами сети и сопутствующими таблицами VLAN, IP-адресов и портов подключения оборудования.

![*Таблица IP*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab3/report/image/8.png){#fig:008 width=30%}

## 

![*Таблица портов*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab3/report/image/9.png){#fig:009 width=70%}

## 

![*Физические устройства сети с номерами портов (Layer 1)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab3/report/image/11.png){#fig:010 width=70%}

## 

![*Схема VLAN сети (Layer 2)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab3/report/image/10.png){#fig:011 width=70%}

## 

![*Схема маршрутизации сети (Layer 3)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab3/report/image/12.png){#fig:012 width=70%}

## 

Сделала аналогичный план адресного пространства для сети 192.168.0.0/16 с соответствующей схемой сети и сопутствующей таблицой IP-адресов.

![*Таблица IP*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab3/report/image/13.png){#fig:013 width=40%}

## 

![*Схема маршрутизации сети (Layer 3)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab3/report/image/14.png){#fig:014 width=70%}


# Вывод

Я познакомилась с принципами планирования локальной сети организации.


