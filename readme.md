Samples for cross account logs exports

1st Setup the S3 access logs part

2nd Deploy Kinesis section which will generate a cloudwatch logs destination

3rd deploy VPC with sample RDS/Ec2 to generate logs which you can then use with kinesis to stream those logs from cloud watch to the destination account


![alt text](https://github.com/bquintas/cross_account_log_exports/blob/master/CrossAccountExportLogs.drawio.png?raw=true)