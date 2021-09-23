# Security Manager

### Security Manager microservice will be responsible for authenticating the user and providing them JWT.
For first time run, make sure to create database **security_manager** first and change credentials as well.

If configurations are same as the repository ones, then curl command to retrieve JWT:

`curl --location --request POST 'http://localhost:8085/oauth/token' \
--header 'Content-Type: application/x-www-form-urlencoded' \
--header 'Authorization: Basic Y2xpZW50OnNlY3JldA==' \
--header 'Cookie: JSESSIONID=9E41DC0312213DC0467B61E45FEC5E67' \
--data-urlencode 'username=admin@TEST01.com' \
--data-urlencode 'password=password' \
--data-urlencode 'grant_type=password'`

