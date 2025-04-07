---
## Front matter
lang: ru-RU
title: "Презентация по лабораторной работе №9"
subtitle: "Дисциплина: Администрирование локальных сетей"
author:
  - Лобанова П.И.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 7 апреля 2025

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

Изучение возможностей протокола STP и его модификаций по обеспечению отказоустойчивости сети, агрегированию интерфейсов и перераспределению нагрузки между ними.

# Задание

1. Сформируйте резервное соединение между коммутаторами msk-donskayasw-1 и msk-donskaya-sw-3.

2. Настройте балансировку нагрузки между резервными соединениями.

3. Настройте режим Portfast на тех интерфейсах коммутаторов, к которым подключены серверы.

4. Изучите отказоустойчивость резервного соединения.

5. Сформируйте и настройте агрегированное соединение интерфейсов Fa0/20 – Fa0/23 между коммутаторами msk-donskaya-sw-1 и msk-donskaya-sw-4.

6. При выполнении работы необходимо учитывать соглашение об именовании.

# Выполнение

![*Логическая схема локальной сети с резервным соединением*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab9/report/image/1.png){#fig:001 width=70%}

##

![*Активация портов в транковом режиме*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab9/report/image/2.png){#fig:002 width=50%}

![*Активация портов в транковом режиме*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab9/report/image/3.png){#fig:003 width=50%}

![*Активация портов в транковом режиме*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab9/report/image/4.png){#fig:004 width=50%}

##

![*Пингование*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab9/report/image/5.png){#fig:005 width=70%}

## 

![*Режим симуляции*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab9/report/image/6.png){#fig:006 width=70%}

## 

На коммутаторе msk-donskaya-sw-2 посмотрела состояние протокола STP для vlan 3.

![*Информация, связанная с протоколом STP*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab9/report/image/7.png){#fig:007 width=70%}


## 

![*Настройка корневого коммутатаора*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab9/report/image/8.png){#fig:008 width=70%}

## 

![*Режим симуляции*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab9/report/image/9.png){#fig:009 width=70%}

## 

![*Настройка режима Portfast*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab9/report/image/10.png){#fig:010 width=50%}

![*Настройка режима Portfast*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab9/report/image/11.png){#fig:011 width=50%}

## 

![*Пингование*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab9/report/image/12.png){#fig:012 width=70%}

## 

Переключила коммутаторы режим работы по протоколу Rapid PVST+.

![*Режим работы по протоколу Rapid PVST+*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab9/report/image/13.png){#fig:013 width=70%}


## 

![*Пингование*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab9/report/image/18.png){#fig:018 width=70%}

## 

Сформировала агрегированное соединение интерфейсов Fa0/20 – Fa0/23 между коммутаторами msk-donskaya-sw-1 и msk-donskaya-sw-4.

![*Логическая схема локальной сети с агрегированным соединением*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab9/report/image/19.png){#fig:019 width=70%}

## 

![*Настройка агрегирования каналов*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab9/report/image/20.png){#fig:020 width=70%}

![*Настройка агрегирования каналов*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab9/report/image/21.png){#fig:021 width=70%}


# Вывод

Я изучила возможности протокола STP и его модификаций по обеспечению отказоустойчивости сети, агрегированию интерфейсов и перераспределению нагрузки между ними.


