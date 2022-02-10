# terraform-eks-template
terraform-eks-demo

# Context
This reposity is highly inspired from this article
https://learn.hashicorp.com/tutorials/terraform/eks?in=terraform/kubernetes

# GIT
### Prerequisites
    cat version.txt  
    echo "0.0.1" > version.txt  
    version=`cat version.txt`  
    message="*yourmessage*"
    
### Push your changes into into the SAMI GIT folder
    git add *  
    git status  
    git commit -a -m "Version $version - $message"  
    git tag -a $version -m "Version $version - $message"  
    git push && git push --tags  
    
### Update Puppetfile into the repository r10k

# TERRAFORM
## Set the env variables
    export AWS_ACCOUNT=<VALUE>
    export AWS_ACCESS_KEY_ID=<VALUE>
    export AWS_SECRET_ACCESS_KEY=<VALUE>
    export AWS_DEFAULT_REGION="us-east-1"
## Run a plan 
    terraform plan -out=out.tfplan
## Apply the plan
    terraform apply out.tfplan
