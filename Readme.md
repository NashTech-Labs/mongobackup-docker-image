The above template will help you to create a mongo backup docker image which can be run as a container in K8s and help to backup your mongodb data.

#### What does the repository contain?

Dockerfile: The dockerfile is used to create the docker image of the mongo backup .

mongobackup.sh: This file is the script which has a function for taking backup of mongo from the host where it is deployed and will take a backup of all the data of database.



#### Variables used in script

AWS_REGION: It defines the aws region that will be defined in your environment where this image will run.

MONGODB_HOST: This defines the mongodb host .

DATABASES: The database name that needs to be backuped

MONGODB_ROOTADMIN_PASSWORD: The mongodb root password.

### How to run this tempalte.

Step 1: First run the below command in the below directory

`docker build -t imagename:tag .`

After this the image will be build and then further that image can be used as a deployment and would be run as a container to backup the mongo data.