# status 
![Progress Actions Status](https://github.com/fendijatmiko/bmi-calculator-python/actions/workflows/python-app.yml/badge.svg)
# Simple App | Body-Mass Index (BMI)
Exercise to make program Body-Mass Index (BMI) with Flask in Python. :D
<pre>
# Test Result | 06 Agustus 2022
</pre>
   forked repo: ***https://github.com/FendiJatmiko/bmi-calculator-python***
## AutoDeployment CI/CD with github action hosted in heroku with 3 env :
   1. dev environment with docker-compose 
         to  run the program: 
         1. clone this repo
         2. install docker & docker compose
         3. run the docker compose `docker-compose up`
         4. then, access it with `curl localhost/?height=167&weight=70`
   2. Staging that can be accessed in : 
      `curl https://staging-cicd-sekolahmu.herokuapp.com/?height=167&weight=70`
   3. Prod environment that can be accessed : 
      `curl https://cicd-sekolahmu.herokuapp.com/?height=167&weight=70`

 minus: 
    didnt install ELK stack and centralized log because i dont have machine with public ip
