# Configure a AWS profile named crossplane
# This ask for the access key, access secret, default region and cli output format
aws configure --profile crossplane

# set a variable with the profile name
AWS_PROFILE=crossplane

# Create a configuration file with profile created
echo -e "[$AWS_PROFILE]\naws_access_key_id = $(aws configure get aws_access_key_id --profile $AWS_PROFILE)\naws_secret_access_key = $(aws configure get aws_secret_access_key --profile $AWS_PROFILE)" > aws-credentials.conf

# Create kubernetes secret from the configuration file
kubectl create secret generic aws-credentials -n crossplane-system --from-file=creds=./aws-credentials.conf