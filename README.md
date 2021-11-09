# terraform-eks-demo
terraform-eks-demo

# This reposity is highly inspired from this article
https://faun.pub/automate-provisioning-of-kubernetes-clusters-on-aws-with-terraform-61ff6aaf8ead

# GIT
## Prerequisites
    cat version.txt  
    echo "0.0.1" > version.txt  
    version=`cat version.txt`  
    message="*yourmessage*"
    
    ## 1. Push your changes into into the SAMI GIT folder
    git add *  
    git status  
    git commit -a -m "Version $version - $message"  
    git tag -a $version -m "Version $version - $message"  
    git push && git push --tags  
    
    ## 2. Update Puppetfile into the repository r10k
