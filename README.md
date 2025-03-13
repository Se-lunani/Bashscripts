# BashScripts - S3 & CloudFormation Automation

This repository contains Bash scripts for managing Amazon S3 buckets and automating AWS CloudFormation stack deployments. These scripts were created as part of my preparation for the **AWS Solutions Architect Associate** exam, where I explored S3 and Infrastructure as Code (IaC) automation using Bash scripting.

I leveraged AWS documentation and guidance from **Andrew Brown (FreeCodeCamp)** to develop these scripts.

## Scripts Overview

### S3 Management Scripts
- **Create-Bucket** – Creates a new S3 bucket.  
- **Delete-Bucket** – Deletes an S3 bucket.  
- **List-Bucket** – Lists all available S3 buckets.  
- **Latest-Bucket** – Retrieves details of the most recently created S3 bucket.  
- **Put-Bucket** – Uploads a bucket configuration.  
- **Put-Object** – Uploads an object (file) to S3.  
- **Delete-Object** – Deletes a specific object from S3.  
- **DeleteAll-Objects** – Deletes all objects in a bucket.  
- **Sync** – Synchronizes a local folder with an S3 bucket.  

### CloudFormation (IaC) Scripts
- **Deploy-IaC** – Deploys a CloudFormation stack using `template.yaml` from the IaC repository.  
- **Delete-IaC** – Deletes the CloudFormation stack deployed by `template.yaml`.  

### Additional Notes
- **Genfiles** – A directory that stores generated test files.  
- **Evan** – A sample file used for object upload testing.  

Enjoy exploring these scripts!
