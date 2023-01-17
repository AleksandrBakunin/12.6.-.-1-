# Домашнее задание к занятию "`12.6. «Репликация и масштабирование. Часть 1»`" - `Александр Бакунин`

---

### Задание 1

Основными различиями, отличающими master-slave (m-s) и master-master (m-m) репликации, являются:
1) В случае m-s репликации данные изначально записываются в master сервер, там же происходят все операции с данными. Slave является вспомогательным сервером, который копирует данные с master'а, однако мы не можем записываться туда напрямую, оттуда мы можем только списать данные. 

2) В случае m-m данные записываются напрямую в оба master'a и могут быть записаны/считаны оттуда в равной степени, то есть это по сути тот же m-s, только каждый сервер является и мастером, и слейвом одновременно.

---

### Задание 2

![alt text](https://github.com/AleksandrBakunin/SQL_Replication_1/blob/main/img/%D0%A0%D0%B5%D0%BF%D0%BB%20%D0%B8%20%D0%BC%D0%B0%D1%81%D1%88%20%D1%87.1.PNG)


Сконфигурированные master и slave машины, репликация работает, ошибок нет.



![alt text](https://github.com/AleksandrBakunin/SQL_Replication_1/blob/main/img/%D0%A0%D0%B5%D0%BF%D0%BB%20%D0%B8%20%D0%BC%D0%B0%D1%81%D1%88%20%D1%87.1%20-%202.PNG)


Конфигурационные файлы my.cnf мастер и слейв серверов.
