FROM python:3
ENV PYTHONUNBUFFERED=1
WORKDIR /api
COPY requirements.txt .
RUN pip install --upgrade pip
RUN pip3 install -r requirements.txt
RUN pip install django django-cors-headers
COPY . /app
EXPOSE 8000
CMD ["python", "manage.py", "runserver"]
