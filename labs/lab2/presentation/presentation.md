---
## Front matter
lang: ru-RU
title: "Презентация по лабораторной работе №2"
subtitle: "Дисциплина: Администрирование локальных сетей"
author:
  - Лобанова П.И.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 20 февраля 2025

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

Получить основные навыки по начальному конфигурированию оборудования Cisco.

# Задание

1. Сделать предварительную настройку маршрутизатора:

– задать имя в виде «город-территория-учётная_записьтип_оборудования-номер»;

– задать интерфейсу Fast Ethernet с номером 0 ip-адрес 192.168.1.254 и маску 255.255.255.0, затем поднять интерфейс;

– задать пароль для доступа к привилегированному режиму (сначала в открытом виде, затем — в зашифрованном);

– настроить доступ к оборудованию сначала через telnet, затем — через ssh;

– сохранить и экспортировать конфигурацию в отдельный файл.

##

2. Сделать предварительную настройку коммутатора:

– задать имя в виде «город-территория-учётная_записьтип_оборудования-номер»;

– задать интерфейсу vlan 2 ip-адрес 192.168.2.1 и маску 255.255.255.0, затем поднять интерфейс;

– привязать интерфейс Fast Ethernet с номером 1 к vlan 2;

– задать в качестве адреса шлюза по умолчанию адрес 192.168.2.254;

– задать пароль для доступа к привилегированному режиму (сначала в открытом виде, затем — в зашифрованном);

– настроить доступ к оборудованию сначала через telnet, затем — через ssh;

– для пользователя admin задать доступ 1-го уровня по паролю;

– сохранить и экспортировать конфигурацию в отдельный файл.

# Выполнение

![*Конфигурация маршрутизатора*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/presentation/image/преза/1.png){#fig:001 width=70%}

## Настройка маршрутизатора

![*Конфигурация маршрутизатора*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/presentation/image/преза/2.png){#fig:002 width=70%}


## Настройка маршрутизатора

![*Конфигурация маршрутизатора*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/presentation/image/преза/3.png){#fig:003 width=70%}


## Проверка подключения

![*Команда ping*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/5.png){#fig:004 width=70%}

## Проверка подключения

![*Подключение через telnet*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/7.png){#fig:005 width=70%}

![*Подключение через telnet*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/10.png){#fig:006 width=70%}

## Проверка подключения

![*Подключение через ssh*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/13.png){#fig:007 width=70%}

## Настройка коммутатора

![*Конфигурация коммутатора*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/presentation/image/преза/4.png){#fig:008 width=70%}

## Настройка коммутатора

![*Конфигурация коммутатора*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/presentation/image/преза/5.png){#fig:009 width=70%}

## Настройка коммутатора

![*Конфигурация коммутатора*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/presentation/image/преза/6.png){#fig:010 width=70%}

## Проверка подключения

![*Команда ping*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/18.png){#fig:011 width=40%}

## Проверка подключения

![*Подключение через telnet*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/22.png){#fig:012 width=70%}

## Проверка подключения

![*Подключение через ssh*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab2/report/image/25.png){#fig:013 width=70%}


# Вывод 

Получить получила основные навыки по начальному конфигурированию оборудования Cisco.
