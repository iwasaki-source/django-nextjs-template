FROM python:3.11

# RUN apt-get update && apt-get install -y \
#   libpq-dev gcc && \
#   apt-get clean

WORKDIR /app

COPY requirements.txt /app/
RUN pip install -r requirements.txt

COPY . /app/

CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]