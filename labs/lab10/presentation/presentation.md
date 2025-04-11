---
## Front matter
lang: ru-RU
title: "Презентация по лабораторной работе №10"
subtitle: "Дисциплина: Администрирование локальных сетей"
author:
  - Лобанова П.И.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 11 апреля 2025

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

Освоить настройку прав доступа пользователей к ресурсам сети.

# Задание

1. Требуется настроить следующие правила доступа:

1) web-сервер: разрешить доступ всем пользователям по протоколу HTTP через порт 80 протокола TCP, а для администратора открыть доступ по протоколам Telnet и FTP;

2) файловый сервер: с внутренних адресов сети доступ открыт по портам для общедоступных каталогов, с внешних — доступ по протоколу FTP;

3) почтовый сервер: разрешить пользователям работать по протоколам SMTP и POP3 (соответственно через порты 25 и 110 протокола TCP), а для администратора — открыть доступ по протоколам Telnet и FTP;

## 

4) DNS-сервер: открыть порт 53 протокола UDP для доступа из внутренней сети;

5) разрешить icmp-сообщения, направленные в сеть серверов;

6) запретить для сети Other любые запросы за пределы сети, за исключением администратора;

7) разрешить доступ в сеть управления сетевым оборудованием только администратору сети.

2. Требуется проверить правильность действия установленных правил доступа.

3. Требуется выполнить задание для самостоятельной работы по настройке прав доступа администратора сети на Павловской.

4. При выполнении работы необходимо учитывать соглашение об именовании.

# Выполнение

![*Размещение ноутбука администратора в сети other-donskaya-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/1.png){#fig:001 width=70%}

## 

![*Конфигурация ноутбука*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/2.png){#fig:002 width=50%}

![*Конфигурация ноутбука*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/3.png){#fig:003 width=50%}

##

![*Настройка доступа к web-серверу*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/4.png){#fig:004 width=70%}

## 

![*Добавление списка управления доступом к интерфейсу*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/5.png){#fig:005 width=70%}

## 

![*Дополнительный доступ для администратора по протоколам Telnet и FTP*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/6.png){#fig:006 width=70%}

## 

![*Доступ по протоколу FTP*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/7.png){#fig:007 width=70%}

## 

![*Доступ по протоколу FTP*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/8.png){#fig:008 width=70%}

## 

![*Настройка доступа к файловому серверу*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/9.png){#fig:009 width=70%}

## 

![*Настройка доступа к почтовому серверу*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/10.png){#fig:010 width=70%}

## 

![*Настройка доступа к DNS-серверу*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/11.png){#fig:011 width=70%}

## 

![*Доступность web-сервера (через браузер) по ip-адресу*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/12.png){#fig:012 width=70%}

## 

![*Доступность web-сервера (через браузер) по имени*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/13.png){#fig:013 width=70%}

## 

![*Разрешение icmp-запросов*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/14.png){#fig:014 width=70%}

## 

![*Список контроля доступа*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/15.png){#fig:015 width=70%}

## 

![*Настройка доступа для сети Other*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/16.png){#fig:016 width=70%}

## 

![*Настройка доступа администратора к сети сетевого оборудования*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/17.png){#fig:017 width=70%}

## 

![*Проверка корректность установленных правил доступа с dk-donskaya-pilobanova-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/18.png){#fig:018 width=70%}

## 

![*Проверка корректность установленных правил доступа с dep-donskaya-pilobanova-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/19.png){#fig:019 width=70%}

## 

![*Проверка корректность установленных правил доступа с admin*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/20.png){#fig:020 width=70%}

## 

![*Размещение ноутбука администратора в сети other-pavlovskaya-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/21.png){#fig:021 width=70%}

## 

![*Настройка доступа для администратора из сети Other на Павловской*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/22.png){#fig:022 width=70%}

## 

![*Проверка корректность установленных правил доступа с admin-pavlovskaya*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/23.png){#fig:023 width=70%}

# Вывод

Я освоила настройку прав доступа пользователей к ресурсам сети.


