FROM python:3.12-alpine
WORKDIR /app

ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1
ENV PIP_ROOT_USER_ACTION=ignore
ENV FLASK_APP=app.py
ENV FLASK_DEBUG=1

COPY requirements.txt app.py /app/

RUN pip install -r requirements.txt

EXPOSE 5000
ENTRYPOINT [ "python3" ]
CMD [ "app.py" ]
