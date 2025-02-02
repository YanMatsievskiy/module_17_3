# Домашнее задание по теме "Миграции. Библиотека alembic."

Цель: усвоить новые правила структурирования проекта с использованием FastAPI. Научиться создавать миграции и подтверждать их при помощи alembic.

Задача "Миграции alembic":

1. Установите все необходимые библиотеки для дальнейшей работы: alembic.

2. Инициализируйте alembic, у вас должна получится следующая структура:

![image](https://github.com/user-attachments/assets/92212c77-feb0-4640-b08f-d41f5cbef9a5)

3. Укажите адрес вашей базы данных 'sqlite:///taskmanager.db' в alembic.ini

4. В env.py импортируйте модели Base, User и Task. Целевой укажите Base.metadata

5. После чего сгенерируйте первую миграцию при помощи alembic revision. Должна появится версия миграции и база данных:

![image](https://github.com/user-attachments/assets/658b5ad6-a8d2-4b71-86c3-92c2bb790e39)

6. Откройте появившуюся базу данных в DB Browser, создастся только 1 таблица - для версий миграций:

![image](https://github.com/user-attachments/assets/d7db7335-a6c2-4ec4-9e74-cdef74de2127)

7. Выполните команду alembic upgrade head, которая позволит вам применить последнюю миграцию и создать таблицы User, Task и запись текущей версии миграции:

![image](https://github.com/user-attachments/assets/189f2c1d-63da-4a03-98a3-dfd00e4f9f4c)

![image](https://github.com/user-attachments/assets/a3a49bd3-37cb-4826-aac9-5ffe372e8a90)

![image](https://github.com/user-attachments/assets/310374f6-0d96-419a-88e8-cf75d1eb7cb9)

Таким образом вы создадите базу данных и 3 реальных таблицы, с данными которых сможете работать в след. домашних заданиях.
