FROM python:3.8.12-bullseye

COPY . .

RUN pip3 install --upgrade pip

RUN pip3 install -r requirements.txt

EXPOSE 8000

RUN python manage.py makemigrations

RUN python manage.py migrate

RUN python manage.py runserver
