web: python manage.py migrate contenttypes --noinput && python manage.py migrate auth --noinput && python manage.py migrate --noinput && python manage.py collectstatic --noinput && gunicorn FSD.wsgi:application --bind 0.0.0.0:$PORT --workers 1 --threads 1 --timeout 120 --max-requests 200 --max-requests-jitter 50

