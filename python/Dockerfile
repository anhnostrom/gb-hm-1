FROM python:3.9.5-alpine3.13
RUN pip install click==7.1.2 Flask==1.1.2 itsdangerous==1.1.0 Jinja2==2.11.2 MarkupSafe==1.1.1 Werkzeug==1.0.1
ADD . /app
EXPOSE 8080
ENTRYPOINT python /app/app.py
