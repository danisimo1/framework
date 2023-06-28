# bumbo web framework (особеноости запуска на Windows)
### подготовка к работе 
```console
cd "/c/Users/User/Desktop/Учёба/Магистратура/1 курс/2 семестр/Елисеев/bumbo-github/bumbo-framework/webapp"
```

Создадим виртуальное окружение:
```console
python3 -m venv venv
```

Вместо Gunicorn используем Waitress WSGI web server

Установка Waitress:
```console
pip install waitress
```

### запуск проекта
Активируем виртуальное окружение:
```console
source venv/Scripts/activate
```

Запускаем Waitress WSGI web server:
```console
waitress-serve --listen=*:8000 app:app
```

