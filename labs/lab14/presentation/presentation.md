---
## Front matter
lang: ru-RU
title: "Презентация по лабораторной работе №14"
subtitle: "Дисциплина: Администрирование локальных сетей"
author:
  - Лобанова П.И.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 1 мая 2025

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

Настроить взаимодействие через сеть провайдера посредством статической маршрутизации локальной сети организации с сетью основного здания, расположенного в 42-м квартале в Москве, и сетью филиала, расположенного в г. Сочи.

# Задание

1. Настроить связь между территориями.

2. Настроить оборудование, расположенное в квартале 42 в Москве.

3. Настроить оборудование, расположенное в филиале в г. Сочи.

4. Настроить статическую маршрутизацию между территориями.

5. Настроить статическую маршрутизацию на территории квартала 42 в г. Москве.

6. Настроить NAT на маршрутизаторе msk-donskaya-gw-1.

7. При выполнении работы необходимо учитывать соглашение об именовании.


# Выполнение

![*Настройка интерфейсов коммутатора provider-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/1.png){#fig:001 width=50%}

## 

![*Настройка интерфейсов маршрутизатора msk-donskaya-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/2.png){#fig:002 width=70%}


## 

![*Настройка интерфейсов маршрутизатора msk-q42-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/3.png){#fig:003 width=70%}

## 

![*Настройка интерфейсов коммутатора sch-sochi-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/4.png){#fig:004 width=70%}

##

![*Настройка интерфейсов маршрутизатора sch-sochi-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/5.png){#fig:005 width=70%}

## 

![*Настройка интерфейсов маршрутизатора msk-q42-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/6.png){#fig:006 width=70%}

## 

![*Настройка интерфейсов коммутатора msk-q42-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/7.png){#fig:007 width=70%}

## 

![*Настройка интерфейсов маршрутизирующего коммутатора msk-hostel-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/8.png){#fig:008 width=70%}

##

![*Настройка интерфейсов коммутатора msk-hostel-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/9.png){#fig:009 width=70%}

## 

![*Настройка интерфейсов маршрутизатора sch-sochi-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/10.png){#fig:010 width=70%}

## 

![*Настройка интерфейсов коммутатора sch-sochi-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/11.png){#fig:011 width=70%}

## 

![*Настройка маршрутизатора msk-donskaya-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/12.png){#fig:012 width=70%}

![*Настройка маршрутизатора msk-q42-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/13.png){#fig:013 width=70%}

## 

![*Настройка маршрутизатора sch-sochi-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/14.png){#fig:014 width=70%}

![*Настройка маршрутизатора msk-q42-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/15.png){#fig:015 width=70%}

## 

![*Настройка интерфейсов маршрутизирующего коммутатора msk-hostel-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/16.png){#fig:016 width=70%}

## 

![*Настройка NAT на маршрутизаторе msk-donskaya-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab14/report/image/17.png){#fig:017 width=70%}

# Вывод

Я настроила взаимодействие через сеть провайдера посредством статической маршрутизации локальной сети организации с сетью основного здания, расположенного в 42-м квартале в Москве, и сетью филиала, расположенного в г. Сочи.

