# Deploying and Testing a Model using Amazon SageMaker Studio V2

## Project Overview

This project focuses on deploying and testing a machine learning model using Amazon SageMaker Studio, integrating multiple AWS services to create a robust and scalable architecture. The project guides you through the entire process, from defining the model to testing it using a web application.

## Services Used

- **Amazon CloudFront**
- **Amazon S3**
- **Amazon API Gateway**
- **AWS Lambda**
- **Amazon SageMaker Endpoint**
- **Amazon SageMaker Notebook**
- **SageMaker Model**
- **Web App**

## Project Structure

### 1. Define the Model

In this initial step, we define a machine learning model using Amazon SageMaker Notebook. The model is trained and prepared for deployment.

### 2. Deploy the Model in Amazon SageMaker Inference Endpoint

Once the model is defined and trained, it's deployed to an Amazon SageMaker Inference Endpoint. This service allows for real-time predictions and can scale based on demand.

![Deploy the Model](https://raw.githubusercontent.com/KireetiChennuru/Deploying-and-Testing-a-Model-using-Amazon-Sage-Maker-Studio-/main/projectimages/Deploy%20the%20model%20in%20Amazon%20SageMaker%20Inference%20Endpoint.jpg "Deploying the Model in Amazon SageMaker Inference Endpoint")

### 3. Test the Deployed Model

After deployment, the model is tested to ensure it performs as expected. Testing involves invoking the endpoint and reviewing the predictions to validate accuracy and performance.

### 4. Creating Endpoint Test Functions in AWS Lambda

AWS Lambda functions are created to interact with the deployed model. These functions handle the logic for invoking the SageMaker Endpoint and processing the responses.

### 5. Updating General Configuration and Environment Variables

Configurations and environment variables are updated across the services to ensure seamless integration and communication between AWS resources.

### 6. Creating S3 Buckets

Amazon S3 buckets are created to store various assets, such as model artifacts, input data, and output results. These buckets are also configured for access by other services in the architecture.

### 7. Creating CloudFront Distributions

Amazon CloudFront distributions are set up to serve the content securely and quickly, leveraging the global edge network.

### 8. Creating API Gateway and Reviewing Resources and Stages to Invoke URL

An API Gateway is created to serve as the entry point for the web application to interact with the deployed model via the Lambda functions and SageMaker endpoint.

### 9. Use Sample Web Application Using Distribution Domain Name and API Gateway URL and Generate Output by Giving Prompts

A sample web application is deployed using the CloudFront distribution domain name and API Gateway URL. The application generates output by interacting with the deployed model based on user-provided prompts.

## Conclusion

This project demonstrates the power of integrating various AWS services to deploy, test, and serve a machine learning model. The architecture ensures scalability, security, and efficiency, making it a solid foundation for deploying production-level AI solutions.
