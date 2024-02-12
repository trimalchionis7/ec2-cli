# Cmd to track status of instance
aws ec2 describe-instances --instance-ids $INSTANCE

# Cmd to retrieve name of instance file
aws ec2 describe-instances --instance-ids $INSTANCE --query 'Reservations[].Instances[].State.Name' --output text