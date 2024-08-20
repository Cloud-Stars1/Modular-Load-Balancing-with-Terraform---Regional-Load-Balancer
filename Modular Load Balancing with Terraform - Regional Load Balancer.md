# Modular Load Balancing with Terraform - Regional Load Balancer || GSP191

## Solution [here](https://youtu.be/M_-C96PEMwk)

### Run the following Commands in the Cloud shell


```
export REGION=
```

```
gcloud auth list

git clone https://github.com/GoogleCloudPlatform/terraform-google-lb
cd ~/terraform-google-lb/examples/basic

export GOOGLE_PROJECT=$(gcloud config get-value project)


sed -i 's/us-central1/'"$REGION"'/g' variables.tf


export TF_VAR_project_id=$DEVSHELL_PROJECT_ID

terraform init
terraform plan
yes | terraform apply --auto-approve
```



### Congratulations 🎉 for completing the Lab !

##### You Have Successfully Demonstrated Your Skills And Determination.

#### *Well done!*

#### Don't Forget to Join the [Telegram Channel](https://t.me/cloudstars24)

### Subscribe to our YouTube Channel [CLOUD STARS](https://www.youtube.com/@cloud-stars)
