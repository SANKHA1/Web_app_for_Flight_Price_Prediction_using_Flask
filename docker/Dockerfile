# init a base image (Alpine is small Linux distro)
FROM python:3.6.1-alpine
# define the present working directory
WORKDIR /Flight-Fare-Prediction-using-Machine-Learning-master
# copy the contents into the working dir
ADD . /Flight-Fare-Prediction-using-Machine-Learning-master
# run pip to install the dependencies of the flask app
RUN pip install --upgrade pip
find -name "requirements.txt"
COPY requirements.txt /tmp
WORKDIR /tmp
RUN pip install -r requirements.txt
# define the command to start the container
CMD ["python","app.py"]