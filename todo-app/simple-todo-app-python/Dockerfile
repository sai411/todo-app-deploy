FROM python:alpine3.17
RUN mkdir my-app
WORKDIR my-app
RUN pip install Django
COPY . $WORKDIR
RUN python3 manage.py makemigrations && python3 manage.py migrate
CMD "python3" "manage.py" "runserver" "0.0.0.0:8000"