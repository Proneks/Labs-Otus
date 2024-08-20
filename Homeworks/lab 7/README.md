# Лабораторная работа. Развертывание коммутируемой сети с резервными каналами

## Топология

![](1.PNG)

## Таблица адресации

| Устройство    | Интерфейс   | IP-адрес  | Маска подсети 
|-----------------|---------------|-------------------------|-------------------|
| S1 | VLAN 1  | 192.168.1.1  |   255.255.255.0   |
| S2 | VLAN 1  | 192.168.1.2 |    255.255.255.0  |
| S3 | VLAN 1  | 192.168.1.3 |    255.255.255.0  | 

### Задачи

Часть 1. Создание сети и настройка основных параметров устройства

Часть 2. Выбор корневого моста

Часть 3. Наблюдение за процессом выбора протоколом STP порта, исходя из стоимости портов

Часть 4. Наблюдение за процессом выбора протоколом STP порта, исходя из приоритета портов

## Решение

# Часть 1. Создание сети и настройка основных параметров устройства

## Шаг 1. Создайте сеть согласно топологии.

![](1.PNG)

## Шаг 2. Настройте базовые параметры каждого коммутатора.

* Отключите поиск DNS

![](2.PNG)

* Присвойте имена устройствам в соответствии с топологией.

![](3.PNG)

* Назначьте class в качестве зашифрованного пароля доступа к привилегированному режиму.

![](4.PNG)

* Назначьте cisco в качестве паролей консоли и VTY и активируйте вход для консоли и VTY каналов.

![](5.PNG)

* Настройте logging synchronous для консольного канала.

![](6.PNG)

* Настройте баннерное сообщение дня (MOTD) для предупреждения пользователей о запрете несанкционированного доступа.

![](7.PNG)

* Задайте IP-адрес, указанный в таблице адресации для VLAN 1 на всех коммутаторах.

![](8.PNG)

* Скопируйте текущую конфигурацию в файл загрузочной конфигурации.

![](9.PNG)