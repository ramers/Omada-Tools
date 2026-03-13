FROM python:3

WORKDIR /usr/src/app

# Копируем файл из той же папки, где лежит Dockerfile
COPY webhookd/requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

# Копируем всё содержимое папки webhookd
COPY webhookd/ ./

CMD [ "python", "./webhookd.py", "--fg" ]
