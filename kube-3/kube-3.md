
# Задание 1: Создание Deployment с двумя контейнерами  
1. Создание Deployment с двумя контейнерами - `kubectl apply -f multitool-pod.yam`  
![kube3-1-deplman](https://github.com/user-attachments/assets/68f55f2d-c40b-446f-aae4-e2b21c53c86f)  
![kube3-2-kgp](https://github.com/user-attachments/assets/5465fe38-1bd7-4504-92b9-dde175ee8fce)  

2. Увеличение количества реплик - `kubectl scale deployment nginx-multitool --replicas=2`  ![kube3-2-kgp](https://github.com/user-attachments/assets/6e5249fc-e61c-4c16-98e5-9e8c0a308469)  
![kube3-3-replica](https://github.com/user-attachments/assets/e92f30ab-bfbe-4330-8bbc-1e22e0b30f9a)  

3. Демонстрация количества подов - `kubectl get pods`  ![kube3-4-rep](https://github.com/user-attachments/assets/13e441dd-d1c1-4dc8-a20f-bb5274f1fd63)  

4. Создание Service - `kubectl apply -f nginx-multitool-service.yaml`  ![kube3-5-svc](https://github.com/user-attachments/assets/84767042-7f63-4ca9-af98-0cfdddceb8b8)  
![kube3-6-svcm](https://github.com/user-attachments/assets/2b25743d-576d-4fd9-9c24-f6532dba998c)  

5. Создание отдельного Pod с multitool и проверка доступа   ![kube3-7-podm](https://github.com/user-attachments/assets/7390b905-c631-4250-a04c-b02cc9ecb960)  
![kube3-8-check](https://github.com/user-attachments/assets/f4d47421-b572-41a4-8f0e-43caa5df9280)  


---
# Задание 2: Deployment с Init-контейнером и зависимостью от Service  
1. Создание Deployment с Init-контейнером   ![kube3-10-repairinitm](https://github.com/user-attachments/assets/fec25359-eaa4-4a0a-8a94-3ba46ada9eb2)

2. Проверка состояния пода до создания сервиса  ![kube3-9-init](https://github.com/user-attachments/assets/de9b3438-d2f1-4d1f-bf6c-b24c1ff46b99)  

3. Создание и запуск Service  
![kube3-11-0-servicein](https://github.com/user-attachments/assets/1e027e73-2ba5-45e3-b5a1-9dbc694d02c6)  


4. Проверка состояния пода после создания сервиса ![kube3-11-checkinit](https://github.com/user-attachments/assets/6ec42eb3-825a-4f71-b438-409a32a300b9)  
