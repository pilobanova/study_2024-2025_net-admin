---
## Front matter
lang: ru-RU
title: "Презентация по лабораторной работе №5"
subtitle: "Дисциплина: Администрирование локальных сетей"
author:
  - Лобанова П.И.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 11 марта 2025

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

Получить основные навыки по настройке VLAN на коммутаторах сети.

# Задание 

1. На коммутаторах сети настроить Trunk-порты на соответствующих интерфейсах, связывающих коммутаторы между
собой.

2. Коммутатор msk-donskaya-sw-1 настроить как VTP-сервер и прописать на нём номера и названия VLAN согласно табл. 3.1 из раздела 3.3.

3. Коммутаторы msk-donskaya-sw-2 — msk-donskaya-sw-4, mskpavlovskaya-sw-1 настроить как VTP-клиенты, на интерфейсах указать принадлежность к соответствующему VLAN.

## 

4. На серверах прописать IP-адреса, как указано в табл. 3.2 из раздела 3.3.

5. На оконечных устройствах указать соответствующий адрес шлюза и прописать статические IP-адреса из диапазона соответствующей сети, следуя регламенту выделения ip-адресов.

6. Проверить доступность устройств, принадлежащих одному VLAN, и недоступность устройств, принадлежащих разным VLAN.

7. При выполнении работы необходимо учитывать соглашение об именовании.

# Выполнение 

Используя приведённую ниже последовательность команд, настроила Trunk-порты на соответствующих интерфейсах всех коммутаторов.

![*Настройка Trunk-портов на коммутаторе msk-donskaya-pilobanova-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/1.png){#fig:001 width=70%}

## 

Используя приведённую ниже последовательность команд по конфигурации VTP, настроила коммутатор msk-donskaya-sw-1 как VTP-сервер и прописала на нём номера и названия VLAN.

![*Настройка коммутатора msk-donskaya-pilobanova-sw-1 как VTP-сервер*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/6.png){#fig:006 width=70%}

## 

Используя приведённую ниже последовательность команд по конфигурации диапазонов портов, настроила коммутаторы msk-donskaya-sw-2 — mskdonskaya-sw-4, msk-pavlovskaya-sw-1 как VTP-клиенты и на интерфейсах указала принадлежность к VLAN.

![*Настройка коммутатора msk-donskaya-pilobanova-sw-2 как VTP-клиента*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/7.png){#fig:007 width=70%}

## 

казала статические IP-адреса на оконечных устройствах и серверах.

![*Указание шлюза для серверов*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/11.png){#fig:011 width=70%}

## 

![*Указание IP-адреса для сервера web*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/12.png){#fig:012 width=70%}

## 

![*Указание шлюза для ДК (Донская)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/15.png){#fig:015 width=70%}

## 

![*Указание IP-адреса для ДК (Донская)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/16.png){#fig:016 width=70%}

## 

![*Команда ping*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/27.png){#fig:027 width=70%}

## 

![*Движение пакета к dk-donskaya-pilobanova-1 от dk-pavlovskaya-pilobanova-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/28.png){#fig:028 width=70%}

## 

![*Движение пакета к dk-donskaya-pilobanova-1 от other-pavlovskaya-pilobanova-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab5/report/image/29.png){#fig:029 width=70%}

# Вывод

Я получила основные навыки по настройке VLAN на коммутаторах сети.


