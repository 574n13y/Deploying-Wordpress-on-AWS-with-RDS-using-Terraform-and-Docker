# Deploying-Wordpress-on-AWS-with-RDS-using-Terraform-and-Docker
       Deploying WordPress on AWS with RDS using Terraform, and Docker


## Task
  - Task 1: Create a Terraform script to deploy a Virtual Machine (VM) in a public subnet and deploy the RDS in a private subnet.
  - Task 2: Create a Dockerfile to deploy Wordpress with Apche Webserver and PHP in the same VM.
  - Task 3: Build the Docker image, tag it, and push it to Docker Hub.
  - Task 4: Connect Wordpress container with RDS database.

## Task 1 - Terraform 
  - We can configure it to use your AWS account by setting the AWS_ACCESS_KEY_ID and AWS_SECRET_ACCESS_KEY environmental variables in your terminal. The Terraform CLI will detect the presence of these variables and use them to authenticate with your AWS account.
  - We can create these environmental variables by executing below commands:
    ```
    export AWS_ACCESS_KEY_ID=your_access_key_id
    export AWS_SECRET_ACCESS_KEY=your_secret_access_key
    ```
  - Replace the values of your_access_key_id and your_secret_access_key with your own AWS Access Key ID and Secret Access Key. Once we have successfully created the environmental variables, you should see something like this by running below command.
    ```
    aws configure
    ```
  - create a folder with whatever name you want. Let’s name it ``Terraform``. Inside the ``Terraform`` folder, create a file named provider.tf. The name of the file can be anything, but the extension must be ``.tf``.
  - For AWS provider, copy and paste below code into provider.tf :
  - 
