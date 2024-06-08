FROM python:3.12

ENV PYTHONUNBUFFERED=1

WORKDIR /blogger-api

COPY requirements.txt .
RUN pip install -r requirements.txt

COPY . .

EXPOSE 5000

CMD ["python", "manage.py", "runserver", "0.0.0.0:5000"]