# Задание  1: Подготовка Helm-чарт для приложения

Использована  команда: `helm create my-nginx`.  
За основу взято приложение `Nginx`.  
Все шаблоны и файлы указаны в `kube-10/my-nginx/`  
![kube10-1-helm](https://github.com/user-attachments/assets/de56e3bb-f940-4dc9-b046-7adf1f5cece3) 

---

# Задание 2: Запуск двух версий в разных неймспейсах

1. Запуск несколько копий приложения   
Использованы команды:  
    `helm install nginx-v1 ./my-nginx --namespace app1 --set image.tag=1.21.1`  
    `helm install nginx-v1 ./my-nginx --namespace app1 --set image.tag=1.21.6`  
    `helm install nginx-v3 ./my-nginx --namespace app2 --set image.tag=1.22.0`  
2. Проверка работы приложения  
![kube10-2-check-name](https://github.com/user-attachments/assets/28683a5f-329b-4d30-8e26-e50b30c23386)
