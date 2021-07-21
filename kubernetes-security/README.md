# Выполнено ДЗ №

 - task01 - cоздать Service Account bob, дать ему роль admin в рамках всего кластера, cоздать Service Account dave без доступа к кластеру;
 - task02 - cоздать Namespace prometheus, создать Service Account carol в этом Namespace, дать всем Service Account в Namespace prometheus возможность, делать get, list, watch в отношении Pods всего кластера
 - task03 - Создать Namespace dev. Создать Service Account jane в Namespace dev. Дать jane роль admin в рамках Namespace dev. Создать Service Account ken в Namespace dev. Дать ken роль view в рамках Namespace dev.

## В процессе сделано:
 - Пункт 1:
    написан манифест 01-sa-bob.yaml, 02-sa-dave.yaml;
 - Пункт 2:
    написан манифест 01-ns-prometheus.yaml, 02-sa-prometheus.yaml;
 - Пункт 3:
    написан манифест  

## Как запустить проект:
 - Применить манифесты kubectl apply -f *.yaml

## Как проверить работоспособность:
 - kubectl get pods
 - kubectl get sa

## PR checklist:
 - [ ] Выставлен label с темой домашнего задания
