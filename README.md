# Домашнее задание к занятию 6 "«Репликация и масштабирование. Часть 1»" - `Филон Андрей`  

---

### Задание 1

На лекции рассматривались режимы репликации master-slave, master-master, опишите их различия.
*Ответить в свободной форме.*

<ins>**Ответ:**</ins>

- Master-Slave репликация.  
В этом подходе выделяется один основной сервер базы данных, который называется Master. На нем происходят все изменения в данных (любые запросы MySQL INSERT/UPDATE/DELETE). Slave-сервер постоянно копирует все изменения с Master. С приложения на Slave-сервер отправляются запросы чтения данных (запросы SELECT). Таким образом Master-сервер отвечает за изменения данных, а Slave за чтение.

- Master-Master репликация.  
В этой схеме, любой из серверов может использоваться как для чтения так и для записи.
---

### Задание 2

Выполните конфигурацию master-slave репликации, примером можно пользоваться из лекции.
*Приложите скриншоты конфигурации, выполнения работы: состояния и режимы работы серверов.*

<ins>**Ответ:**</ins>

![1](https://github.com/AndreyFilon/bd-12-06/blob/main/2.%20master-status.jpg)    
![1](https://github.com/AndreyFilon/bd-12-06/blob/main/2.%20slave-config2.jpg)  
![1](https://github.com/AndreyFilon/bd-12-06/blob/main/2.%20slave-config.jpg)  
![1](https://github.com/AndreyFilon/bd-12-06/blob/main/2.%20slave-status.jpg)
![1](https://github.com/AndreyFilon/bd-12-06/blob/main/1.jpg)   

---
