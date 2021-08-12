# awslambda_ssl_expiry

# Monitor SSL Certificate Expiry Using AWS Lambda

To getting the alerts and take necessary steps to renew the SSL certificates of a domain.
Using AWS Lambda service to monitor SSL Certificates expiry to get warning/critical alerts based on the days left.

# Services Used To Monitor SSL Certificate:
```bash
  1.AWS Lambda — We can run code without provisioning servers 
  2.AWS Cloud watch — Cloud watch Events to schedule the lambda job 
  3.AWS SNS — To get alerts based on warning/critical days.
```

# Setup

```bash
1. Login to AWS console and open the SNS dashboard.
2. Create an SNS topic to get the alerts.
3. To get the emails we need to subscribe(add) the email address in the topic created above.
4. Go to Lambda Service Dashboard and Create the function then select the Author from scratch(Lambda>Functions>Create function>Author from scratch)
5. Create a Schedule event using CloudWatch to call the above Lambda function on daily basis.


```
