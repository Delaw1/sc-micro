# sc-micro
a small microservice node-express project

This is a microservice application to be used to send sms to 2000 numbers, consisting of two services: authService and smsService. The authService acts as the gateway. a "POST: /sms" endpoint expects email, password and messageBody inputs. The edpoints validates if the email == "aaa@example.com" and password == "password". If this condition is true, it sends the data to the smsService microservice. The smsService reciees this and uses twilio to send e massage cosisting of the email address the sender used in authenticating and the messageBody, to an assumed list of 200 phone numbers. 

It's purpose is simply to play around with microservices. Not entirely functional
