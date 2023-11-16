web: gunicorn -b 0.0.0.0:$PORT --name redash -w 4 redash.wsgi:app
worker: celery worker --app=redash.worker --beat -Qqueries,scheduled_queries,celery
