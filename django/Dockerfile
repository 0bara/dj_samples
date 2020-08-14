FROM python:3.7-alpine

WORKDIR /opt/app
COPY requirements.txt ./
RUN pip install --upgrade pip \
	&& pip install --no-cache-dir -r ./requirements.txt

EXPOSE 8000
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
