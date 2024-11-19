---
title: MikroTik
sidebar_position: 6
---

Роутеры MikroTik используют операционную систему с открытым исходным кодом RouterOS, которая предоставляет услуги маршрутизации, беспроводных сетей и фаервола для домашних и небольших офисных сетей.

## Настройте DNS-over-HTTPS

1. Перейдите в настройки роутера MikroTik:
   - Откройте браузер и перейдите по IP-адресу вашего роутера (обычно это `192.168.88.1`)
   - Для подключения к роутеру MikroTik вы также можете использовать Winbox
   - Введите имя пользователя и пароль администратора
2. Импортируйте корневой сертификат:
   - Скачайте последний пакет доверенных корневых сертификатов: [https://curl.se/docs/caextract.html](https://curl.se/docs/caextract.html)
   - Перейдите в _Файлы_. Нажмите _Загрузить_ и выберите загруженный пакет сертификатов cacert.pem
   - Перейдите в _Система_ → _Сертификаты_ → _Импорт_
   - В поле _Имя файла_ выберите загруженный файл сертификатов
   - Нажмите _Импортировать_
3. Настройте DNS-over-HTTPS:
   - Перейдите в _IP_ → _DNS_
   - В разделе _Серверы_, добавьте следующие серверы AdGuard DNS:
     - `94.140.14.49`
     - `94.140.14.59`
   - Установите для параметра _Разрешить удалённые запросы_ значение _Да_ (это необходимо для работы DNS-over-HTTPS)
   - В поле _Использовать сервер DoH_ введите URL частного сервера AdGuard DNS: `https://d.adguard-dns.com/dns-query/*******`
   - Нажмите _ОK_
4. Создайте статические записи DNS:
   - В _Настройках DNS_, нажмите _Статический_
   - Нажмите _Добавить_
   - Установите _Имя_ как d.adguard-dns.com
   - Установите _Тип_ как A
   - Установите _Адрес_ как `94.140.14.49`
   - Установите _Время жизни_ как 1д 00:00:00
   - Повторите процесс для создания идентичной записи, но установите _Адрес_ на `94.140.14.59`
5. Отключите Peer DNS на DHCP-клиенте:
   - Перейдите в _IP_ → _DHCP Client_
   - Дважды щёлкните по клиенту, используемому для подключения к интернету (обычно это интерфейс WAN)
   - Снимите флажок _Использовать Peer DNS_
   - Нажмите _ОK_
6. Привяжите свой IP-адрес.
7. Проверьте получившееся:
   - Возможно, вам потребуется перезагрузить роутер MikroTik, чтобы все изменения вступили в силу
   - Очистите кеш DNS вашего браузера. Вы можете использовать инструмент, такой как [https://www.dnsleaktest.com](https://www.dnsleaktest.com/) для проверки того, находятся ли ваши DNS-запросы теперь в маршруте через AdGuard

## Через панель управления роутера

Используйте эту инструкцию, если ваш роутер Keenetic не поддерживает настройку DNS-over-HTTPS или DNS-over-TLS:

1. Откройте панель управления роутера. Доступ возможен по адресам `192.168.1.1` или `192.168.0.1`.
2. Введите логин пользователя администратора (обычно это admin) и пароль роутера.
3. Откройте _Webfig_ → _IP_ → _DNS_.
4. Выберите _Серверы_ и введите один из следующих адресов DNS-серверов.
   - IPv4: `94.140.14.49` и `94.140.14.59`
   - IPv6: `2a10:50c0:0:0:0:0:ded:ff` и `2a10:50c0:0:0:0:0:dad:ff`
5. Сохраните настройки.
6. Привяжите свой IP (или ваш выделенный IP, если у вас есть подписка Team).

- [Выделенные IP-адреса](/private-dns/connect-devices/other-options/dedicated-ip.md)
- [Привязанные IP-адреса](/private-dns/connect-devices/other-options/linked-ip.md)