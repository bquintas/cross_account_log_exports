These 2 templates help deploy Cloudtrail logs from a "sender" account to a S3 bucket in a "receiver" account. Does not have to be in the same AWS Organization.


1st - The receiver account obtains the AWS account Id of the sender and deploys the stack cloudtrail_receiver_account.yaml in the receiver account 
2nd - After the receiver stack is deployed the receiver needs to provide the S3 bucket name, Prefix and TrailName that the sender should use.
3rd - The sender deploys cloudtrail_sender_account.yaml using the bucket name , Prefix and Trail name provided by the receiver.