# aws-aurora-serverless-rds
**To launch Aurora Serverless RDS Instance in AWS Cloud**

Navigate to AWS RDS console - select - create a database

![image](https://github.com/kohlidevops/aws-aurora-serverless-rds/assets/100069489/640eb21a-f3f7-49f1-83cf-c66dc1c6843a)

I select Engine version as default one and it should be a Production templates. Because we have more options than Dev/Test templates.

![image](https://github.com/kohlidevops/aws-aurora-serverless-rds/assets/100069489/8cab0755-7638-4d1e-a43d-14d7c50d7d02)

Provide database identifier name and strong credentials to ensure highly secure.

![image](https://github.com/kohlidevops/aws-aurora-serverless-rds/assets/100069489/4437971f-fb43-4702-9c0e-110e7a69f921)

![image](https://github.com/kohlidevops/aws-aurora-serverless-rds/assets/100069489/664dd1ef-a9f9-4091-bb2e-1f82a1bcdc86)

I'm going to use burstable class to save cost.

In Availability and Durability, I will go with "Create an Aurora Replica or Reader node in different AZ". We know that the data by default is going to be Multi-AZ and durable. But its actually for you to create a Multi-AZ deployment by creating Aurora replica or Reader node in different AZ.

![image](https://github.com/kohlidevops/aws-aurora-serverless-rds/assets/100069489/774da79d-3708-43e0-98eb-91425be5bb2e)

I just leave this as default and will go with default VPC

![image](https://github.com/kohlidevops/aws-aurora-serverless-rds/assets/100069489/f5182bce-36e6-4338-b1da-181c50a4fda8)

![image](https://github.com/kohlidevops/aws-aurora-serverless-rds/assets/100069489/5d8f423b-8208-46db-9e14-676b9f5c74cd)

Backup retention would be between 1 and 35 days and going to encrypt the database with KMS key.

![image](https://github.com/kohlidevops/aws-aurora-serverless-rds/assets/100069489/3bc0b08f-2be6-4f62-a410-b05f17575b53)

You can able to export any logs to CloudWatch Loggroups and enable auto-minor version upgrade if you really want.

![image](https://github.com/kohlidevops/aws-aurora-serverless-rds/assets/100069489/194c4751-e7d3-48c4-ad01-366ff5f70c9d)

We good to go to create a Aurora RDS instance.

You can able to see the reader, writer and regional cluster in RDS console for Aurora serverless. 

![image](https://github.com/kohlidevops/aws-aurora-serverless-rds/assets/100069489/08585ffe-84c1-4ab9-9ce3-1d0832c53f70)

So, the reader and writes has different end points to work on it. 

![image](https://github.com/kohlidevops/aws-aurora-serverless-rds/assets/100069489/4e872627-6bef-42b7-b5e6-2db20ff7787f)

You can setup replica Auto-scaling with Action button to select create replica auto-scaling

![image](https://github.com/kohlidevops/aws-aurora-serverless-rds/assets/100069489/58ef6f50-cf14-4614-8763-e92ea53ce9dd)

That's it.













