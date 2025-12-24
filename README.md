
# Laba1-Pi_432
# ОТЧЁТ ПО ЛАБОРАТОРНОЙ РАБОТЕ №1
## Работа с Docker, Dockerfile и Docker Compose

---

## ФИО и группа 

*Султанаева Рената, Малышев Михаил*  
*ПИ-430Б*

---

# Ход выполнения работы

---

## 1. Изучение теоретической части

Были изучены:
- основные команды Docker;
- структура Dockerfile;
- назначение Docker Compose.


---

## 2. Установка Docker Desktop

На компьютер установлен Docker Desktop, содержащий Docker Engine и Docker Compose.

<img width="1898" height="992" alt="Снимок экрана 2025-11-08 115549" src="https://github.com/user-attachments/assets/a90736d9-bc0d-4561-a694-5855c4416316" />


---

## 3. Создание проекта Flask

В рабочей директории созданы файлы:
- app.py
- requirements.txt
  
<img width="1046" height="756" alt="Снимок экрана 2025-11-08 131807" src="https://github.com/user-attachments/assets/46ef2c03-6ba0-443e-b01a-2c3d474ffc32" />
<img width="352" height="92" alt="Снимок экрана 2025-11-08 131816" src="https://github.com/user-attachments/assets/a90ae7a2-567b-4eeb-bf7d-7e0ed85c0d1b" />

---

## 4. Создание Dockerfile

Создан Dockerfile для сборки образа приложения.

<img width="672" height="382" alt="Снимок экрана 2025-11-08 131944" src="https://github.com/user-attachments/assets/af43c25a-7435-4d76-ba44-56a645d04d55" />

---

## 5. Создание docker-compose.yml

Создан docker-compose.yml.

<img width="688" height="740" alt="Снимок экрана 2025-11-08 132209" src="https://github.com/user-attachments/assets/3d1e399b-f3cd-4b50-91aa-8c5530eda904" />

---

## 6. Запуск

Образ собран командой:
docker build -t myapp:1.0 .
Прописываем docker compose up --build. Первая часть команды запускает все сервисы, создаёт контенеры, а вторая - пересобирает все образы прописанные в build:.

<img width="1194" height="237" alt="Снимок экрана 2025-11-08 132401" src="https://github.com/user-attachments/assets/00c1e189-8233-41bf-acb3-7e8b3e1f82f5" />

---

## 7. Открываем localhost

<img width="1252" height="277" alt="2025-11-08_13-44-01" src="https://github.com/user-attachments/assets/c71c54e9-00e1-475e-b52e-052d111b2ab8" />

---

## Заключение

В ходе лабораторной работы были изучены команды Docker и Docker Compose, созданы и запущены контейнеры Flask и PostgreSQL.  
Были решены конфликты портов и ошибки аутентификации.  

В результате:  
- Flask-приложение успешно подключено к PostgreSQL.  
- Получен практический опыт сборки образов и запуска многосервисных приложений через Docker Compose.  
- Освоены методы отладки контейнеров и проброса портов.  

Работа показала эффективность Docker для развёртывания переносимых приложений.
