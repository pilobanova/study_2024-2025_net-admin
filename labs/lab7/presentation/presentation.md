---
## Front matter
lang: ru-RU
title: "Презентация по лабораторной работе №7"
subtitle: "Дисциплина: Администрирование локальных сетей"
author:
  - Лобанова П.И.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 20 марта 2025

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

Получить навыки работы с физической рабочей областью Packet Tracer, а также учесть физические параметры сети.

# Задание 

Требуется заменить соединение между коммутаторами двух территорий msk-donskaya-sw-1 и msk-pavlovskaya-sw-1 на соединение, учитывающее физические параметры сети, а именно —   расстояние между двумя территориями.
При выполнении работы необходимо учитывать соглашение об именовании.

# Выполнение 

![*Физическая рабочая область Packet Tracer*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab7/report/image/1.png){#fig:001 width=50%}

## 

![*Изображение зданий в физической рабочей области Packet Tracer*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab7/report/image/2.png){#fig:002 width=70%}

## 

![*Размещение в физической рабочей области Packet Tracer серверной с подключением оконечных устройств (сеть территории «Донская»)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab7/report/image/3.png){#fig:003 width=70%}

## 

![*Отображение серверных стоек в Packet Tracer*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab7/report/image/4.png){#fig:004 width=70%}

## 

![*Размещение в физической рабочей области Packet Tracer серверной с подключением оконечных устройств (сеть территории «Павловская»)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab7/report/image/5.png){#fig:005 width=70%}

## 

![*Пингование*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab7/report/image/6.png){#fig:006 width=70%}

## 

![*Активирование разрешения на учет физических характеристик среды передачи*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab7/report/image/7.png){#fig:007 width=70%}

## 

![*Расстояние между двумя территориями*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab7/report/image/8.png){#fig:008 width=70%}

## 

![*Пингование*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab7/report/image/10.png){#fig:009 width=70%}

## 

![*Схема сети с повторителями*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab7/report/image/11.png){#fig:010 width=70%}

## 

Заменила имеющиеся модули на PT-REPEATERNM-1FFE и PT-REPEATER-NM-1CFE для подключения оптоволокна и витой пары по технологии Fast Ethernet.

![*Повторитель с портами PT-REPEATER-NM-1FFE и PT-REPEATER-NM-1CFE на территории Донская*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab7/report/image/12.png){#fig:011 width=70%}

## 

![*Повторитель с портами PT-REPEATER-NM-1FFE и PT-REPEATER-NM-1CFE на территории Павловская*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab7/report/image/13.1.png){#fig:012 width=70%}

## 

![*Размещение в физической рабочей области Packet Tracer серверной с подключением оконечных устройств (сеть территории «Павловская»)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab7/report/image/14.png){#fig:013 width=70%}

## 

Подключила коммутатор msk-donskaya-sw-1 к msk-donskaya-mc-1 по витой паре, msk-donskaya-mc-1 и msk-pavlovskaya-mc-1 — по оптоволокну, msk-pavlovskaya-sw-1 к msk-pavlovskaya-mc-1 — по витой паре.

![*Схема сети с учётом физических параметров сети в логической рабочей области Packet Tracer*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab7/report/image/15.png){#fig:014 width=50%}


## 

![*Пингование*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab7/report/image/16.png){#fig:015 width=70%}

# Вывод

Я получила навыки работы с физической рабочей областью Packet Tracer, а также учла физические параметры сети.


