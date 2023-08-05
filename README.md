# Kittygram - социальная сеть для любителей котиков. 
###### Let's make kitty greate again!!!

___

### Описание

Данная платформа предназначена для владельцев котиков, самих еотиков и любителей наблюдать за жизнбю котиков. Соблюдаем правила, лайкаем котов и уважаем других пользователей. 
Основные задачи платформы:

😸 Пости любимого кота. 

😻 ️Подписывайся на других пользователей и комментируй его котиков. 

😸 Мяу!


___

### Используемые инструменты. 

[Python] - backend target language

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)

[Django Rest Framework] - Python toolkit for building Web APIs

![DjangoREST](https://img.shields.io/badge/DJANGO-REST-ff1709?style=for-the-badge&logo=django&logoColor=white&color=ff1709&labelColor=blue)

[JavaScript] - frontend target language

![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)

[React] - JavaScript library for building user interfaces

![React](https://img.shields.io/badge/react-%2320232a.svg?style=for-the-badge&logo=react&logoColor=%2361DAFB)

[Ubuntu] - open source operating system based on Linux

![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
 
[Gunicorn] - Python WSGI HTTP Server for UNIX

![Gunicorn](https://img.shields.io/badge/gunicorn-%298729.svg?style=for-the-badge&logo=gunicorn&logoColor=white)

[Nginx] - HTTP and reverse proxy server

![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white)

___

### Как запустить проект. 

✅ Придумай и зарегистрируй доменное имя. 

✅ Зупасти сервер в GitBush (или иной консоли). 

✅ Установа npm

```
npm install и npm run build
```

✅ Установка Nginx

```
sudo apt install nginx
```

✅ Клонирование репозитория. 

```
git clone
```

✅ Создаем и активируем виртуальное окруженеие. 

```
python3 -m venv venv
sourse venv/bin/activate
```

✅ Установка зависимостей. 

```
python -m pip install --upgrade pip
pip install -r requirements.txt
```

✅ Создание файла для переменных окружения

```
touch .env

```

✅ Выполнение миграций и создание суперпользователя

```
python manage.py migrate
python manage.py createsuperuser
```


✅ Собираем статистику бэкенда

```
python manage.py collectstatic
```

✅ Работа с фронтэндом

```
cd ../frontend
npm i
```

✅ Сбор статистики фронтэнда. 

```
npm run build
```

✅ Установка и создание файла Gunicorn_kittygram

```
sudo nano /etc/systemd/system/gunicorn_kittygram.service
```

```
sudo systemctl status gunicorn
```


✅ Копирование статистики фронэнда и бэкенда. 

```
sudo cp -r /home/<system-username>/Kittygram_Social_Network/frontend/build/. /var/www/Kittygram_Social_Network/
sudo cp -r /home/<system-username>/Kittygram_Social_Network/backend/static_backend/ /var/www/Kittygram_Social_Network/
```

✅ Создание солкальной рабочей папки 

```
cd /var/www/
sudp mkdir kittygram
cd kittygram
sudo mkdir media
sudo chown -R <system-username> /var/www/kittygram/media/
```

✅ Работа и управление Nginx

```
sudo nano /etc/nginx/sites-enabled/default
sudo ufw allow 'Nginx Full'
sudo ufw allow OpenSSH
sudo ufw enable
```

✅ Запуск Nginx

```
sudo systemctl start nginx
```

✴️  Работа с SSL сертификатом и программой certbot

```
sudo apt install snapd
sudo snap install core; sudo snap refresh core
sudo snap install --classic certbot
sudo ln -s /snap/bin/certbot /usr/bin/certbot
sudo certbot --nginx
```

___


Create by [Jar1sh]
