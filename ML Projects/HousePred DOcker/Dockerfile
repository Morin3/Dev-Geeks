FROM python:3.14.0a3-alpine3.20 
COPY . /app
WORKDIR /app
RUN pip install -r requirements.txt
EXPOSE $PORT
CMD guincorn --workers=4 --bind 0.0.0.0:$PORT app:app
```