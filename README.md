# Face_Recognition_Project
Face Recognition using Aws Services

# My AWS-powered Face Recognition Project

This repository contains the code for my AWS-powered Face Recognition project. The project details and insights can be found in my LinkedIn blog: [https://www.linkedin.com/feed/update/urn:li:activity:7093626711338102785/].

## Project Overview
...


Commands 

❖ Install Aws Shell : 
          
          pip install aws-shell

❖ Configure Aws :

          aws configure
          
❖ Create a collection on aws rekognition :

        aws rekognition create-collection --collection-id facerecognition_collection --region ap-south-1

❖ Create table on DynamoDB :

          aws dynamodb create-table --table-name facerecognition \
          --attribute-definitions AttributeName=RekognitionId,AttributeType=S \
          --key-schema AttributeName=RekognitionId,KeyType=HASH \
          --provisioned-throughput ReadCapacityUnits=1,WriteCapacityUnits=1 \
          --region ap-south-1
❖ Create S3 bucket :

          aws s3 mb s3://bucket-name --region ap-south-1
          
  
        
         
