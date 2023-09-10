# vitkazak_platform
vitkazak Platform repository

# Выполнено ДЗ №1

 - [+] Основное ДЗ
 - [+] Задание со *

## В процессе сделано:
 - Установка на виртуалку под ОС Linux (Ubuntu 22.04) kubectl, docker, minikube
 - Установлен dashboard для minikube, ознакомился с его интерфейсом и возможностями
 - Установлен k9s, ознакомился с его интерфейсом и возможностями
 - Проверил перезапуск подов в namespace kube-system. Посмотрел разнве механизмы перезапуска данных подов чрез kubectl describe
 - Был собран образ веб-сервера nginx через Dockerfile, учитывая все требования из задания и выложен в публичный репо как vitkazak/k8s-webserver:latest
 - Написан манифест web-pod.yaml с init-контейнером
 - Запустил приложение и получил локально к нему доступ через kubectl port-forward а также через kube-forwarder
![Снимок экрана от 2023-09-10 15-58-25](https://github.com/otus-kuber-2023-08/vitkazak_platform/assets/31851694/71f77f95-9f86-402c-8034-eee173cf2e4c)
 - Собран образ hipstershop frontend и выложен на Docker Hub как vitkazak/hipster-frontend:v0.0.1
 - Запустил через ad-hoc команду

## Задание со *
 - Причиной, по которой падал pod frontend, было отсутствие переменных окружения, необходимых для работы приложения.
 - Создан манифест kubernetes-intro/frontend-pod-healthy.yaml, в котором для контейнера frontend указаны необходимые переменные окружения.
   
![Снимок экрана от 2023-09-10 15-59-37](https://github.com/otus-kuber-2023-08/vitkazak_platform/assets/31851694/b81e41b2-3cda-4679-817b-9d14c2d36c85)


## Как запустить проект:
 - Например, запустить команду X в директории Y

## Как проверить работоспособность:
 - Например, перейти по ссылке http://localhost:8080

## PR checklist:
 - [ ] Выставлен label с темой домашнего задания
