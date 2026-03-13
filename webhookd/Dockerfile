FROM python:3

WORKDIR /usr/src/app

# Копируем requirements.txt из той же папки
COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt

# Копируем все остальные файлы из текущей папки
COPY . .

CMD [ "python", "./webhookd.py", "--fg" ]
