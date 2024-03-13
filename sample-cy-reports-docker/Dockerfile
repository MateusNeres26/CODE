FROM cypress/base:latest

WORKDIR /home/cypress/


RUN apt-get clean && apt-get update && apt-get install -f


COPY . /home/cypress/

VOLUME [ "/home/cypress/allure-report" ]

RUN npm install

CMD ["npm", "run", "test:allure"]