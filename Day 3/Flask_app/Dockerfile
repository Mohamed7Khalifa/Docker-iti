FROM python:3.7-alpine
WORKDIR /code
ENV FLASK_APP=app.py\
    FLASK_RUN_HOST=0.0.0.0
COPY requirements.txt requirements.txt
RUN pip install -r requirements.txt && \
        apk add --no-cache gcc musl-dev linux-headers
EXPOSE 5000
COPY . .
CMD ["flask", "run"]