FROM python:3.10

# Working Directory
WORKDIR /app

# Copy source code to working directory
COPY ./ /app/

# Install packages from requirements.txt

RUN pip3 install --no-cache-dir --upgrade pip &&\
    pip3 install --no-cache-dir -r requirements.txt

# Expose container port
EXPOSE 80

CMD [ "python3", "app.py" ]