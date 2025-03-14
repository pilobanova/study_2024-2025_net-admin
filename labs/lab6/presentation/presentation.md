---
## Front matter
lang: ru-RU
title: "Презентация по лабораторной работе №6"
subtitle: "Дисциплина: Администрирование локальных сетей"
author:
  - Лобанова П.И.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 14 марта 2025

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

Настроить статическую маршрутизацию VLAN в сети.

# Задание 

1. Добавить в локальную сеть маршрутизатор, провести его первоначальную настройку.

2. Настроить статическую маршрутизацию VLAN.

3. При выполнении работы необходимо учитывать соглашение об именовании.

# Выполнение 

![*Схема сети*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab6/report/image/1.png){#fig:001 width=70%}

## 

Сконфигурировала маршрутизатор, задав на нём имя, пароль для доступа к консоли, настроила удалённое подключение к нему по ssh.

![*Начальная настройка маршрутизатора*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab6/report/image/2.png){#fig:002 width=50%}

## 

![*Настройка порта на коммутаторе*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab6/report/image/3.png){#fig:003 width=70%}

## 

На интерфейсе f0/0 маршрутизатора msk-donskaya-pilobanova-gw-1 настроила виртуальные интерфейсы, соответствующие номерам VLAN. Согласно таблице IP-адресов задала соответствующие IP-адреса на виртуальных интерфейсах.

![*Настройка интерфейсов маршрутизатора*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab6/report/image/4.png){#fig:004 width=50%}

## 

![*Команда ping для разных vlan*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab6/report/image/6.png){#fig:006 width=70%}

## 

![*Передвижение пакета ICMP*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab6/report/image/7.png){#fig:007 width=70%}

# Вывод

Я настроила статическую маршрутизацию VLAN в сети.
