# Домашнее задание к занятию «Kubernetes. Причины появления. Команда kubectl»

1. `microk8s status --wait-ready`  Проверяет состояние MicroK8s и ожидает, пока все компоненты не станут "готовы".  
![kube1-1](https://github.com/user-attachments/assets/5d183fc1-129e-4449-a795-7614c849961d)  

2. microk8s enabled dashboard -   Включает веб-интерфейс Kubernetes Dashboard и необходимые компоненты
![kub1-2-dashen](https://github.com/user-attachments/assets/6672bef5-49a2-41e2-a153-03a0a9b1d4b5)   

3. alias kubectl='microk8s kubectl' -  Создаёт псевдоним, чтобы можно было писать просто `kubectl`, не указывая `microk8s`.  

4. nano /var/snap/microk8s/current/certs/csr.conf.template` Редактирование шаблона генерации сертификатов MicroK8s .  
![kube1-3-csr](https://github.com/user-attachments/assets/cee70e08-584e-49d4-a5b1-33e8f5ca3377)

6. `microk8s refresh-certs --cert front-proxy-client.crt` - Обновляет указанный сертификат 
![kube1-4-cert](https://github.com/user-attachments/assets/93da6042-ac29-4678-bed9-beda1a52d509)  

7. `sudo systemctl stop ufw`  Отключает фаервол UFW, чтобы не блокировал сетевые соединения.  

8. Установка kubectl
![kube1-5-kubectlin](https://github.com/user-attachments/assets/828f0488-d560-4c58-ab1a-33cff9a3daa2)  

9. nano dashboard-admin.yaml`   Создание YAML-файла с ролью `dashboard-admin`.  
![kube1-6-dash-adm](https://github.com/user-attachments/assets/db96e285-bda3-4aad-9416-31d2a635464f)

10. `kubectl apply -f dashboard-admin.yaml`  Применение этой конфигурации — создание аккаунта и привязки роли к нему.

11. `microk8s kubectl port-forward -n kube-system services/kubernetes-dashboard 10443:443 --address 192.168.0.13` - проброс портов на внешний IP  
![kube1-8portfor](https://github.com/user-attachments/assets/d0747f82-d303-4eaa-a789-b43c60ff6240)  

12.  `microk8s kubectl -n kube-system get secret microk8s-dashboard-token -o jsonpath="{.data.token}" | base64 --decode` - получение токена для входа в dashboard
![kube1-9takecert](https://github.com/user-attachments/assets/a8d385cd-2e9b-4d2c-95db-a55c92227310)


**Dashboard**  
 
![kube1-10dash](https://github.com/user-attachments/assets/c6e68bfd-e0ce-4046-98f3-db253d228ea5)


**Kubectl get nodes**  
![get_nodes](https://github.com/user-attachments/assets/3a1e9739-2162-47a4-b64f-8ca78e39c83f)
