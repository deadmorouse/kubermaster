
# Задание 1: Создание Deployment с двумя контейнерами
1. Создание Deployment с двумя контейнерами - `kubectl apply -f multitool-pod.yam`
2. Увеличение количества реплик - `kubectl scale deployment nginx-multitool --replicas=2`
3. Демонстрация количества подов - `kubectl get pods`
4. Создание Service - `kubectl apply -f nginx-multitool-service.yaml`
5. Создание отдельного Pod с multitool и проверка доступа 

---
# Задание 2: Deployment с Init-контейнером и зависимостью от Service
1. Создание Deployment с Init-контейнером - 
2. Проверка состояния пода до создания сервиса
3. Создание и запуск Service
4. Проверка состояния пода после создания сервиса