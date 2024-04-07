web: gunicorn app:app -b 0.0.0.0:8000
worker: gunicorn app:app -b 0.0.0.0:8001 --workers 3

# Comando para ejecutar un script de inicialización
init: python manage.py createsuperuser

# Comando para ejecutar una tarea de mantenimiento
maintenance: python manage.py collectstatic