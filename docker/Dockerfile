FROM python:3.9


WORKDIR /devops

RUN apt-get update -y && apt-get install git -y && apt-get install python3-pip -y

RUN git clone https://github.com/LondheShubham153/django-notes-app.git


RUN pip install -r django-notes-app/requirements.txt

EXPOSE 8080

CMD [ "python" , "django-notes-app/manage.py", "runserver", "0.0.0.0:8080" ] 
