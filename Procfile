web: newrelic-admin run-program gunicorn -w 5 -b 0.0.0.0:5000 --log-level info --log-file - aleph.manage:app
worker: celery -A aleph.queue worker -c 10 -l INFO --logfile=-