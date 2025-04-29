# Задание 1: Создание Deployment приложения, использующего локальный PV, созданный вручную.  

1. Создание папки на локальной ноде для хранения данных  
2. манифесты для PV и PVC  
![kube7-pvc1](https://github.com/user-attachments/assets/266b50f0-4aba-4bd7-8625-f80e41abdac6)  
![kube7-pv1](https://github.com/user-attachments/assets/1bc95406-cb70-4946-84b0-f1edadbdda92)  

3. Манифест Deployment с двумя контейнерами  
![kube7-dep1](https://github.com/user-attachments/assets/832d535b-44e2-4679-af62-f5091167fa8f)  

4. Проверяем, что все работает  
![kube7-1-get](https://github.com/user-attachments/assets/5751cff3-25d9-48a8-845c-478805368c77)  
![kube7-2-ch](https://github.com/user-attachments/assets/f45707e7-4a3c-48b9-883b-96979fcec60e)  

5. Удаляем Deployment и PVC  
![kub7-3-chdelpvc](https://github.com/user-attachments/assets/0b157060-c859-4a37-9dbc-1d9de101e7d9)  

6. Удалем PV  (поставлено значение Retain -  Данные сохранятся после удаления PVC)  
![kube7-4-pvdel](https://github.com/user-attachments/assets/a297d5de-c01a-44c9-9f74-baf62032bb04)  

---

# Задание 2: Создание Deployment приложения, которое может хранить файлы на NFS с динамическим созданием PV.  

1. Включение и настройка NFS осуществлялось по этому мануалу https://microk8s.io/docs/how-to-nfs  
2. Манифесты StorageClass и PVC  
![kube7-stcl2](https://github.com/user-attachments/assets/994dded2-2aae-4b4e-9230-dd35aeecc142)  
![kube7-pvc2](https://github.com/user-attachments/assets/cbe8ce9c-2303-4d7e-ab31-8ffaa0e75cfc)  

3. Манифест Deployment  
![kube7-depl2](https://github.com/user-attachments/assets/94b8c99c-9784-4e5d-a109-6254196e05d3)  

4. Проверка, что все поднялось  
![kube7-5s-stcl](https://github.com/user-attachments/assets/996ee641-8bee-48f1-a22d-f146cf5c5f1f)  
![kube7-6-pv](https://github.com/user-attachments/assets/ed7de4ca-983b-4553-8df3-c496294de3c5)  

5. Проверка NFS-хранилища  
![kube7-10-checkmnt](https://github.com/user-attachments/assets/20a7b210-e0b2-4edb-b0be-5e5fcb1052fc)

