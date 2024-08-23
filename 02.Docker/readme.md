# Домашнее задание к занятию 4 «Оркестрация группой Docker контейнеров на примере Docker Compose»

## Задача 1

[https://hub.docker.com/repository/docker/nikise/custom-nginx/general](https://hub.docker.com/repository/docker/nikise/custom-nginx/general)

## Задача 2

![task2](https://github.com/SeNike/Study_24/blob/main/02.Docker/task2.png)

## Задача 3
![task3-0.png](https://github.com/SeNike/Study_24/blob/main/02.Docker/task3.0.png)
Когда вы нажимаете Ctrl-C в терминале, где вы подключены к контейнеру, это посылает сигнал прерывания (SIGINT) основному процессу. Если этот процесс завершится, контейнер также завершит свою работу, потому что в Docker основное правило — контейнер работает, пока работает его основной процесс. Как только основной процесс завершается, контейнер переходит в статус "Exited".
![task3-1.png](https://github.com/SeNike/Study_24/blob/main/02.Docker/task3.1.png)

Проблема заключается в том, что после изменения настроек Nginx принимает соединения на 81 порту, а проброшен из контейнера 80.

![task3-2.png](https://github.com/SeNike/Study_24/blob/main/02.Docker/task3.2.png)

## Задача 4

![task4](https://github.com/SeNike/Study_24/blob/main/02.Docker/task4.png)

## Задача 5

![task5-1.png](https://github.com/SeNike/Study_24/blob/main/02.Docker/task5.1.png)
Был запущен файл compose.yaml, т.к. таков синтаксис комманд compose
![task5-2.png](https://github.com/SeNike/Study_24/blob/main/02.Docker/task5.2.png)

![task5-3.png](https://github.com/SeNike/Study_24/blob/main/02.Docker/task5.3.png)
![task5-4.png](https://github.com/SeNike/Study_24/blob/main/02.Docker/task5.4.png)
![task5-5.png](https://github.com/SeNike/Study_24/blob/main/02.Docker/task5.5.png)
Объяснение предупреждения:
Предупреждение сообщает о том, что были найдены "осиротевшие" контейнеры, связанные с проектом. Это контейнеры, которые были созданы предыдущей версией манифеста, но теперь они не соответствуют текущему состоянию или больше не описаны в манифесте.
