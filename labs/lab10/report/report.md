---
## Front matter
title: "Отчет по лабораторной работе №10"
subtitle: "Дисциплина: Администрирование локальных сетей"
author: "Лобанова Полина Иннокентьвна"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Освоить настройку прав доступа пользователей к ресурсам сети.

# Задание

1. Требуется настроить следующие правила доступа:

1) web-сервер: разрешить доступ всем пользователям по протоколу HTTP через порт 80 протокола TCP, а для администратора открыть доступ по протоколам Telnet и FTP;

2) файловый сервер: с внутренних адресов сети доступ открыт по портам для общедоступных каталогов, с внешних — доступ по протоколу FTP;

3) почтовый сервер: разрешить пользователям работать по протоколам SMTP и POP3 (соответственно через порты 25 и 110 протокола TCP), а для администратора — открыть доступ по протоколам Telnet и FTP;

4) DNS-сервер: открыть порт 53 протокола UDP для доступа из внутренней сети;

5) разрешить icmp-сообщения, направленные в сеть серверов;

6) запретить для сети Other любые запросы за пределы сети, за исключением администратора;

7) разрешить доступ в сеть управления сетевым оборудованием только администратору сети.

2. Требуется проверить правильность действия установленных правил доступа.

3. Требуется выполнить задание для самостоятельной работы по настройке прав доступа администратора сети на Павловской.

4. При выполнении работы необходимо учитывать соглашение об именовании.

# Выполнение лабораторной работы

1. В рабочей области проекта подключила ноутбук администратора с именем admin к сети к other-donskaya-1 с тем, чтобы разрешить ему потом любые действия, связанные с управлением сетью. Для этого подсоединила ноутбук к порту 24 коммутатора msk-donskaya-sw-4 и присвоила ему статический адрес 10.128.6.200, указав в качестве gateway-адреса 10.128.6.1 и адреса DNS-сервера 10.128.0.5.

![*Размещение ноутбука администратора в сети other-donskaya-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/1.png){#fig:001 width=70%}

![*Конфигурация ноутбука*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/2.png){#fig:002 width=70%}

![*Конфигурация ноутбука*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/3.png){#fig:003 width=70%}

2. Настроила доступ к web-серверу по порту tcp 80.

![*Настройка доступа к web-серверу*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/4.png){#fig:004 width=70%}

3. Добавила список управления доступом к интерфейсу.

![*Добавление списка управления доступом к интерфейсу*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/5.png){#fig:005 width=70%}

4. Настроила дополнительный доступ для администратора по протоколам Telnet и FTP.

![*Дополнительный доступ для администратора по протоколам Telnet и FTP*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/6.png){#fig:006 width=70%}

5. Убедилась, что с узла с ip-адресом 10.128.6.200 есть доступ по протоколу FTP. 

![*Доступ по протоколу FTP*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/7.png){#fig:007 width=70%}

6. Попробовала провести аналогичную процедуру с другого устройства сети. Убедилась, что доступ будет запрещён.

![*Доступ по протоколу FTP*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/8.png){#fig:008 width=70%}

7. Настроила доступ к файловому серверу.

![*Настройка доступа к файловому серверу*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/9.png){#fig:009 width=70%}

8. Настроила доступ к почтовому серверу.

![*Настройка доступа к почтовому серверу*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/10.png){#fig:010 width=70%}

9. Настроила доступ к DNS-серверу.

![*Настройка доступа к DNS-серверу*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/11.png){#fig:011 width=70%}

10. Проверила доступность web-сервера (через браузер) по ip-адресу и по имени.

![*Доступность web-сервера (через браузер) по ip-адресу*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/12.png){#fig:012 width=70%}

![*Доступность web-сервера (через браузер) по имени*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/13.png){#fig:013 width=70%}

11. Настроила разрешение icmp-запросов.

![*Разрешение icmp-запросов*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/14.png){#fig:014 width=70%}

12. Посмотрела номера строк правил в списке контроля доступа.

![*Список контроля доступа*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/15.png){#fig:015 width=70%}

13. Настроила доступ для сети Other. 

![*Настройка доступа для сети Other*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/16.png){#fig:016 width=70%}

14. Настроила доступ администратора к сети сетевого оборудования.

![*Настройка доступа администратора к сети сетевого оборудования*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/17.png){#fig:017 width=70%}

15. Проверила корректность установленных правил доступа, попытавшись получить доступ по различным протоколам с разных устройств сети к подсети серверов и подсети сетевого оборудования. Пропинговать сервера получилось со всех устройства, а сетевое оборудование только с устройства admin.

![*Проверка корректность установленных правил доступа с dk-donskaya-pilobanova-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/18.png){#fig:018 width=70%}

![*Проверка корректность установленных правил доступа с dep-donskaya-pilobanova-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/19.png){#fig:019 width=70%}

![*Проверка корректность установленных правил доступа с admin*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/20.png){#fig:020 width=70%}

16. Разрешила администратору из сети Other на Павловской действия, аналогичные действиям администратора сети Other на Донской.

![*Размещение ноутбука администратора в сети other-pavlovskaya-1*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/21.png){#fig:021 width=70%}

![*Настройка доступа для администратора из сети Other на Павловской*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/22.png){#fig:022 width=70%}

17. Проверила корректность установленных правил доступа.

![*Проверка корректность установленных правил доступа с admin-pavlovskaya*](/home/pilobanova/work/study/2024-2025/Администрирование локальных сетей/net-admin/net-admin/labs/lab10/report/image/23.png){#fig:023 width=70%}


# Выводы

Я освоила настройку прав доступа пользователей к ресурсам сети.

## Контрольные вопросы

1. Как задать действие правила для конкретного протокола?

Например, permit tcp any host 10.128.0.2 eq 80.

2. Как задать действие правила сразу для нескольких портов?

Для этого нужна команда interface range.

3. Как узнать номер правила в списке прав доступа?

show access −lists

4. Каким образом можно изменить порядок применения правил в списке контроля доступа?

access −list <номера в списке> permit

# Список литературы{.unnumbered}

::: {#refs}
:::
