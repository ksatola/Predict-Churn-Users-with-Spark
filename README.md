# Predict-Churn-Users-with-Spark

https://www.viget.com/articles/set-up-aws-cli-and-download-your-s3-files-from-the-command-line/

How to get data
Install AWS CLI
$ brew install awscli

Get AWS access key
1. Log into the IAM Console.
2. Go to Users.
3. Click on your user name (the name not the checkbox).
4. Go to the Security credentials tab.
5. Click Create access key. Don't close that window yet!
6. You'll see your Access key ID. Click "Show" to see your Secret access key.
7. Download the key pair for safe keeping, add the keys to your password app of choice, or do whatever you do to keep secrets safe. Remember this is the last time Amazon will show this secret access key.

Run aws configure and answer the prompts.
$ aws configure
AWS Access Key ID [None]: <enter the access key you just created>
AWS Secret Access Key [None]: <enter the secret access key you just created>
Default region name [None]: <enter region - valid options are listed below >
Default output format [None]: <format - valid options are listed below >
  
$ aws s3 sync s3://<bucket>/<path> </local/path>
123MB
$ aws s3 cp s3://udacity-dsnd/sparkify/mini_sparkify_event_data.json ~/aws
12GB
$ aws s3 cp s3://udacity-dsnd/sparkify/sparkify_event_data.json ~/aws
