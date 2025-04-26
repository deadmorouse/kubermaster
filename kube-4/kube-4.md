# Задание 1:  Создать Deployment и обеспечить доступ к контейнерам приложения по разным портам из другого Pod внутри кластера
1. Deployment с двумя контейнерами и 3 репликами  
![kube4-1-last](https://github.com/user-attachments/assets/e09b24f8-a27f-49c9-a54b-00eb28110585) 


2. Service для проброса портов  
![kube4-2-service](https://github.com/user-attachments/assets/d0e64670-e527-4ba1-bf06-1e87401d6325)  
![kube4-3-gp](https://github.com/user-attachments/assets/127e211e-b114-4c5a-aae9-d40d938efafe)  

3. Отдельный Pod с multitool для проверки  

4. Проверка доступа через curl  
![kube4-5-checknginx](https://github.com/user-attachments/assets/65ecc28e-fcdb-4ae9-bf99-c14ef23ef803)  

---
# Задание 2: Создать Service и обеспечить доступ к приложениям снаружи кластера  

1. Cоздание Service для nginx (извне)  
![kube4-5-newservice](https://github.com/user-attachments/assets/c91aca1c-9c3b-4d99-ad3f-a56b0a7d571c)  
![kube4-6-checksvc](https://github.com/user-attachments/assets/b0410dc7-abe0-464f-bf80-c524a0602596)  

2. Проверка доступ снаружи  
![kube4-7-checkout](https://github.com/user-attachments/assets/fa706f34-8c08-4109-8543-fad28477de0f) 

