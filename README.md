## Terraform Spike

Spike code to learn terraform.

### How to run

These examples are written to run against AWS.

Create or use a user who has the `AmazonEC2FullAccess` permission.

Either
```
export AWS_ACCESS_ID=<your aws access id>
export AWS_SECRET_ACCESS_KEY=<your aws secret key>
```
OR run
```
aws configure # provide the values for the values prompted
```

Note that the `~/.aws/credentials` file is created

Then, from one of the directories containing `main.tf`, run
```
terraform apply
```

Note the IP address from the step above and then run:

```
curl http://<ip_address_from_above>
```
