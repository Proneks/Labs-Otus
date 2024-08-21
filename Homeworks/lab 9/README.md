# Лабораторная работа - Конфигурация безопасности коммутатора

## Топопология

![](1.jpg)

## Таблица адресации

| Устройство    | interface/vlan   | IP-адрес  | Маска подсети |
|-----------------|---------------|-------------------------|-------------------|
| R1 | G0/0/1   | 192.168.10.1  |   255.255.255.0   | 
| R1 | Loopback 0    | 10.10.1.1 |    255.255.255.0  | 
| S1 | VLAN 10   | 192.168.10.201|    255.255.255.0  | 
| S2 | VLAN 10 | 192.168.10.202 |    255.255.255.0   | 
| PC-A | NIC      | DHCP|    255.255.255.0  | 
| PC-B | NIC      | DHCP |    255.255.255.0  | 
