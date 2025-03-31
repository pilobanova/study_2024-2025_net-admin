---
## Front matter
lang: ru-RU
title: "Презентация по лабораторной работе №8"
subtitle: "Дисциплина: Администрирование локальных сетей"
author:
  - Лобанова П.И.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 31 марта 2025

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

Приобретение практических навыков по настройке динамического распределения IP-адресов посредством протокола DHCP в локальной сети.

# Задание

1. Добавить DNS-записи для домена donskaya.rudn.ru на сервер dns.

2. Настроить DHCP-сервис на маршрутизаторе.

3. Заменить в конфигурации оконечных устройствах статическое распределение адресов на динамическое.

4. При выполнении работы необходимо учитывать соглашение об именовании.

# Выполнение

![*Логическая схема локальной сети с добавленным DNS-сервером*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab8/report/image/1.png){#fig:001 width=70%}

## 

![*Активация порта*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab8/report/image/2.png){#fig:002 width=70%}

## 

![*Конфигурирование dns сервера*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab8/report/image/3.png){#fig:003 width=70%}

## 

![*Конфигурирование dns сервера*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab8/report/image/4.png){#fig:004 width=70%}

## 

![*Настройка сервиса DNS*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab8/report/image/5.png){#fig:005 width=70%}

## 

Настроила DHCP-сервис на маршрутизаторе: указала IP-адрес DNS-сервера; затем перешла к настройке DHCP; задала название конфигурируемому диапазону адресов (пулу адресов), указала адрес сети, а также адреса шлюза и DNS-сервера; задала пулы адресов, исключаемых из динамического распределения.

![*Конфигурирование DHCP-сервиса*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab8/report/image/6.png){#fig:006 width=50%}

## 

![*Изменение адресов*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab8/report/image/9.png){#fig:009 width=70%}

## 

![*Пингование*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab8/report/image/10.png){#fig:010 width=70%}

## 

![*Режим симуляции*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab8/report/image/11.png){#fig:011 width=70%}

## 

![*Информация по DHCP запросу*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab8/report/image/12.png){#fig:012 width=70%}

# Вывод

Я приобрела практические навыки по настройке динамического распределения IP-адресов посредством протокола DHCP в локальной сети.
