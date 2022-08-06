# status 
[![Progress Actions Status](https://github.com/fendijatmiko/bmi-calculator-python/actions/workflows/python-app.yml/badge.svg)]
# Simple App | Body-Mass Index (BMI)
Exercise to make program Body-Mass Index (BMI) with Flask in Python. :D

Rumus:
```
bmi = kg/m^2
```

## Method-1: Run this Program in Localhost
First, you must install some of library in `requirements.txt` using `python-pip`:
```
pip install -r requirements.txt
```
Then, run:
```
python3 app.py
```
Output:
```
 * Serving Flask app "app" (lazy loading)
 * Environment: production
   WARNING: This is a development server. Do not use it in a production deployment.
   Use a production WSGI server instead.
 * Debug mode: off
 * Running on http://0.0.0.0:5000/ (Press CTRL+C to quit)
```

## Method-2: Dockerize this Apps (Run inside Docker Container)
You can dockerize this app with following command, btw i use `python:3.8-alpine`. You can see or custome image in `Dockerfile`:
```
docker build -t bmi:v1 . --no-cache
```
and, Run:
```
docker run -d --rm --name bmi -p 5000:5000 bmi:v1
```

## Verify
To verify the program running, try with accessing the url like this: `http://localhost:5000/?height=167&weight=70` and you can custom value `heigh` and `weight`. If there are bug, please info me. :D

Output:

![result](img/bmi.png)
# Test Result | 06 Agustus 2022
### AutoDeployment CI/CD with github action hosted in heroku with 3 env :
   1. dev environment with docker-compose 
      testing accessing the apps localy: 
      `curl localhost/?height=167&weight=70`
   2. Staging that can be accessed in : 
      `curl https://staging-cicd-sekolahmu.herokuapp.com/?height=167&weight=70`
   3. Prod environment that can be accessed : 
      `curl https://cicd-sekolahmu.herokuapp.com/?height=167&weight=70`
