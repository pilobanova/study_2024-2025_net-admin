---
## Front matter
lang: ru-RU
title: "Презентация по лабораторной работе №12"
subtitle: "Дисциплина: Администрирование локальных сетей"
author:
  - Лобанова П.И.
institute:
  - Российский университет дружбы народов, Москва, Россия
date: 21 апреля 2025

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

Приобретение практических навыков по настройке доступа локальной сети к внешней сети посредством NAT.

# Постановка задачи

Требуется подключить локальную сеть организации к сети Интернет (распределение внешних ip адресов дано в табл. 12.1) с учётом ограничений, накладываемых на определённые подсети локальной сети:

1) сеть управления устройствами не должна иметь доступ в Интернет;

2) оконечные устройства сети дисплейных классов должны иметь доступ только к сайтам, необходимым для учёбы (в данном случае к www.yandex.ru, stud.rudn.university);

3) пользователям из сети кафедр разрешено работать только с образовательными сайтами (в данном случае это esystem.pfur.ru);

4) пользователям сети администрации разрешено работать только с сайтом университета www.rudn.ru;

## 

5) в сети для других пользователей компьютер администратора должен иметь полный доступ во внешнюю сеть, а другие пользователи — не должны выходить в Интернет;

6) ограничения для серверов:

– WEB-сервер должен быть доступен по порту 80;

– почтовый сервер должен быть доступен по портам 25 и 110;

– файловый сервер должен быть доступен извне по портам протокола FTP;

7) компьютер администратора должен быть доступен из внешней сети по протоколу удалённого рабочего стола (Remote Desktop Protocol, RDP).

# Задание

1. Сделать первоначальную настройку маршрутизатора provider-gw-1 и коммутатора provider-sw-1 провайдера: задать имя, настроить доступ по паролю и т.п.

2. Настроить интерфейсы маршрутизатора provider-gw-1 и коммутатора provider-sw-1 провайдера.

3. Настроить интерфейсы маршрутизатора сети «Донская» для доступа к сети провайдера.

4. Настроить на маршрутизаторе сети «Донская» NAT с правилами, указанными в разделе 12.2.

5. Настроить доступ из внешней сети в локальную сеть организации, как указано в разделе 12.2.

6. Проверить работоспособность заданных настроек.

7. При выполнении работы необходимо учитывать соглашение об именовании.

# Выполнение

![*Первоначальная настройка маршрутизатора provider-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab12/report/image/1.png){#fig:001 width=70%}

## 

![*Первоначальная настройка коммутатора provider-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab12/report/image/2.png){#fig:002 width=70%}

## 

![*Настройка интерфейсов маршрутизатора provider-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab12/report/image/3.png){#fig:003 width=70%}

## 

![*Настройка интерфейсов коммутатора provider-sw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab12/report/image/4.png){#fig:004 width=70%}

## 

![*Настройка интерфейсов маршрутизатораmsk-donskaya-gw-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab12/report/image/5.png){#fig:005 width=70%}

## 

![*Настройка пула адресов для NAT*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab12/report/image/6.png){#fig:006 width=70%}

![*Настройка списка доступа для NAT (Сеть дисплейных классов)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab12/report/image/7.png){#fig:007 width=70%}

## 

![*Настройка списка доступа для NAT (Сеть кафедр)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab12/report/image/8.png){#fig:008 width=70%}

![*Настройка списка доступа для NAT (Сеть администрации)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab12/report/image/9.png){#fig:009 width=70%}

## 

![*Настройка списка доступа для NAT (Доступ для компьютера администратора)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab12/report/image/10.png){#fig:010 width=70%}

![*Настройка Port Address Translation*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab12/report/image/11.png){#fig:011 width=70%}

## 

![*Настройка интерфейсов для NAT*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab12/report/image/12.png){#fig:012 width=70%}

## 

![*Настройка доступа из Интернета (WWW-сервер)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab12/report/image/20.png){#fig:013 width=70%}

![*Настройка доступа из Интернета (Файловый сервер)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab12/report/image/13.png){#fig:014 width=70%}


## 

![*Настройка доступа из Интернета (Почтовый сервер)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab12/report/image/14.png){#fig:015 width=70%}

![*Настройка доступа из Интернета ( Доступ по RDP)*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab12/report/image/15.png){#fig:016 width=70%}

## 

![*Проверка работоспособности*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab12/report/image/16.png){#fig:017 width=70%}

## 

![*Проверка работоспособности*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab12/report/image/17.png){#fig:018 width=70%}

## 

![*Проверка работоспособности*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab12/report/image/18.png){#fig:019 width=70%}

## 

![*Проверка работоспособности*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab12/report/image/19.png){#fig:020 width=70%}

# Вывод

Я приобрела практические навыки по настройке доступа локальной сети к внешней сети посредством NAT.

