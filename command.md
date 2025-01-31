# command to create iam user in aws
aws iam create-user --user-name <username>
# command to list out iam users
aws iam list-users
# command to delete iam users in aws using the cli
aws iam delete-user --user-name <username>
# command to create s3 bucket on cli
aws s3api create-bucket --bucket clam-bucket4532 --region us-east-1
# command to delete s3 bucket
 aws s3api delete-bucket --bucket clam-bucket4532 --region us-east-1
 # command to move folder to s3 bucket
 aws s3 mv secret-folder s3://clam-bucket4532 --recursive
# command to move files from s3 bucket to a created folder
 aws s3 mv s3://clam-bucket4532 secret-folder2 --recursive
# command to remove a file from the s3 bucket
 aws s3 rm s3://bam-bucket4532/letter3.txt
 # to remove evrything in an s3 bucket
 aws s3 rm s3://bam-bucket4532 --recursive
 # to create a keypair in cli
 aws ec2 create-key-pair --key-name sandal
# to delete keypair using cli
 aws ec2 delete-key-pair --key-name sandal
# to create or run an ec2 instance using cli
 aws ec2 run-instances --image-id ami-091f18e98bc129c4e --count 1 --instance-type t2.micro --key-name joy --security-group-ids sg-0b49a2e1743b78308 --subnet-id subnet-0aeb09421d2207632
# to describe an ec2 instance using cli
 aws ec2 describe-instances --instance-ids i-024bc6b349451521c
 # to stop an ec2 instance using cli
 aws ec2 stop-instances --instance-ids i-024bc6b349451521c
 # to terminate or delete an ec2 instance
 aws ec2 stop-instances --instance-ids i-024bc6b349451521c