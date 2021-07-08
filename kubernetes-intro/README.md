# Выполнено ДЗ №2
 - Kubelet смотрит состояние подов, и в случае чего, запускает заново;
 - Не при генерации файла yaml не добавило перевенных;

## В процессе сделано:
 - Пункт 1:
    - Уcтановлен kubectl;
    - Установлен minikube;
    - создан Dockerfile, в котором будет описан образ web сервера на nginx;
    - создана дериктория kubernetes-intro/web;
    - собран докер образ и размешен в Container Registry Docker Hub;
    - Написан манифест web-pod.yaml;
    - Собран и запушен образ Hipster Shop
    - Сгенерирован frontend-pod-healthy.yaml

 - Пункт 2

## Как запустить проект:
 - Поместить манифест web-pod.yaml в k8s;
 - Создать pod коммандой kubectl apply -f web-pod.yaml;
 
## Как проверить работоспособность:
 - Открыть порт для pod коммандой: kubectl port-forward --address 0.0.0.0 pod/web 8000:8000
 - Перейти по ссылке http://localhost:8080

## PR checklist:
 - [ ] Выставлен label с темой домашнего задания