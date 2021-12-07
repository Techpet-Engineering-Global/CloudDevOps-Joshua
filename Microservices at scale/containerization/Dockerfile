FROM python:3.7.3-stretch

#working directory
WORKDIR /app

#copy sourcecode to working directory
COPY . flask_app/web.py /app/

#install packages from requirements.txt
RUN pip install --trusted-host pypi.python.org -r requirements.txt

#expose port 80
EXPOSE 80

#run app.py in container launch
CMD ["python", "web.py"]