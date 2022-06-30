# Get project ID 
gcloud projects list --format='value(project_id)'

# Create service account
gcloud iam service-accounts create crossplane-service-account --display-name "crossplane service account" --project=crossplane-330620

# Get the name of the service account
gcloud iam service-accounts list --filter="email ~ ^crossplane-service-account" --format='value(email)'

# Add required IAM role to the service account
gcloud projects add-iam-policy-binding crossplane-330620 --member "serviceAccount:crossplane-service-account@crossplane-330620.iam.gserviceaccount.com" --role="roles/iam.serviceAccountUser"

gcloud projects add-iam-policy-binding crossplane-330620 --member "serviceAccount:crossplane-service-account@crossplane-330620.iam.gserviceaccount.com" --role="roles/cloudsql.admin"

gcloud projects add-iam-policy-binding crossplane-330620 --member "serviceAccount:crossplane-service-account@crossplane-330620.iam.gserviceaccount.com" --role="roles/container.admin"

gcloud projects add-iam-policy-binding crossplane-330620 --member "serviceAccount:crossplane-service-account@crossplane-330620.iam.gserviceaccount.com" --role="roles/redis.admin"

gcloud projects add-iam-policy-binding crossplane-330620 --member "serviceAccount:crossplane-service-account@crossplane-330620.iam.gserviceaccount.com" --role="roles/compute.networkAdmin"

gcloud projects add-iam-policy-binding crossplane-330620 --member "serviceAccount:crossplane-service-account@crossplane-330620.iam.gserviceaccount.com" --role="roles/storage.admin"

# Extract the file and convert it into a base64 string

gcloud iam service-accounts keys create crossplane-service-account.json --iam-account crossplane-service-account@crossplane-330620.iam.gserviceaccount.com

base64 crossplane-service-account.json | tr -d "\n"
