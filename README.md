# AWS-SNS-SMS-OTP API in NodeJS (Express.js)

![aws-sns-otp-api nodejs repo github](./demo/aws-sns-otp-api.png)

![Visitors](https://visitor-badge.glitch.me/badge?page_id=realabbas.aws-sns-otp-api)

### API Endpoint

`GET Request to / route` with following paramaters in the GET Request

- message `String`
- number `String`
- subject `String`

### Setup
- Create an account on AWS
- Navigate to SNS
- Create Security Credentials
- Apply for Extension in Message Limit by contacting customer support in case the OTP fails

### Instructions

Send a GET Request from browser,

`http://localhost:3000/?message=[Message]&number=[Number]&subject=[Subject]`

After triggering the API, you will receive the OTP.

![OTP from AWS SNS API Nodejs](https://dev-to-uploads.s3.amazonaws.com/i/kb75txaszcmtn8g3nqzq.jpg)

The mobile number should be E.164 format but without the + character.

*Example:*

You want to send a message to a number,

The country code is 44

The mobile number is (0)7700 900123

The E.164 format would be +447700900123

Remove the + character

Then Visit 

`http://localhost:3000/?message=my message&number=447700900123&subject=My Subject`
