VPC and Subnet Provisioning
- 3 IPv4 CIDR
- 1 IPv6 CIDR (AWS)
- All subnets created on 1 AZ except for one subnet
- Used for deployment of a workers on 1 AZ for a Network Function
- Default routing to transit gateway


Using CodePipeline: https://github.com/rolvhil/CodePipeline/blob/main/VPC-pipeline.yaml
- The parameters section on the Cloudformation template are parametized as json files. One for test and for prod. Compress all files into .zip, name it as vpc-subnets.zip and upload to S3 bucket - pipeline-bucket-vims-vpc - of the Pipeline

If you plan to use only the Cloudformation yaml file. Please adjust the Parameter section.