---
## Front matter
lang: ru-RU
title: "Презентация по лабораторной работе №15"
subtitle: "Дисциплина: Администрирование локальных сетей"
author:
  - Лобанова П.И.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 13 мая 2025

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

Настроить динамическую маршрутизацию между территориями организации.

# Задание

1. Настроить динамическую маршрутизацию по протоколу OSPF на маршрутизаторах msk-donskaya-gw-1, msk-q42-gw-1, msk-hostel-gw-1, sch-sochi-gw-1.

2. Настроить связь сети квартала 42 в Москве с сетью филиала в г. Сочи напрямую.

3. В режиме симуляции отследить движение пакета ICMP с ноутбука администратора сети на Донской в Москве (Laptop-PT admin) до компьютера пользователя в филиале в г. Сочи pc-sochi-1.

## 

4. На коммутаторе провайдера отключить временно vlan 6 и в режиме симуляции убедиться в изменении маршрута прохождения пакета ICMP с ноутбука администратора сети на Донской в Москве (Laptop-PT admin) до компьютера пользователя в филиале в г. Сочи pc-sochi-1.

5. На коммутаторе провайдера восстановить vlan 6 и в режиме симуляции убедиться в изменении маршрута прохождения пакета ICMP с ноутбука администратора сети на Донской в Москве (Laptop-PT admin) до компьютера пользователя в филиале в г. Сочи pc-sochi-1.

6. При выполнении работы необходимо учитывать соглашение об именовании.

# Выполнение

![*Настройка маршрутизатора msk-donskaya-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab15/report/image/1.png){#fig:001 width=70%}

## 

![*Проверка состояния протокола OSPF на маршрутизаторе msk-donskaya-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab15/report/image/2.png){#fig:002 width=70%}

## 

![*Проверка состояния протокола OSPF на маршрутизаторе msk-donskaya-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab15/report/image/3.png){#fig:003 width=70%}

## 

![*Настройка маршрутизатора msk-q42-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab15/report/image/4.png){#fig:004 width=70%}

## 

![*Настройка маршрутизирующего коммутатора msk-hostel-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab15/report/image/5.png){#fig:005 width=70%}

## 

![*Настройка маршрутизатора sch-sochi-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab15/report/image/6.png){#fig:006 width=70%}

##

![*Настройка интерфейсов коммутатора provider-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab15/report/image/7.png){#fig:007 width=70%}

## 

![*Настройка маршрутизатора msk-q42-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab15/report/image/8.png){#fig:008 width=70%}

## 

![*Настройка коммутатора sch-sochi-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab15/report/image/9.png){#fig:009 width=70%}

## 

![*Настройка маршрутизатора sch-sochi-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab15/report/image/10.png){#fig:010 width=70%}

## 

![*Путь пакета ICMP с ноутбука администратора сети на Донской до компьютера пользователя г. Сочи*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab15/report/image/11.png){#fig:011 width=70%}

## 

![*Отключение vlan 6*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab15/report/image/12.png){#fig:012 width=70%}


## 

![*Путь пакета ICMP с ноутбука администратора сети на Донской до компьютера пользователя г. Сочи*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab15/report/image/13.png){#fig:013 width=50%}


## 

![*Восстановление vlan 6*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab15/report/image/14.png){#fig:014 width=70%}

## 

![*Путь пакета ICMP с ноутбука администратора сети на Донской до компьютера пользователя г. Сочи*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab15/report/image/15.png){#fig:015 width=50%}

# Вывод

Я настроила динамическую маршрутизацию между территориями организации.



