[![CI](https://github.com/nogibjj/aws-template/actions/workflows/cicd.yml/badge.svg?branch=main)](https://github.com/nogibjj/aws-template/actions/workflows/cicd.yml)
[![Codespaces Prebuilds](https://github.com/nogibjj/aws-template/actions/workflows/codespaces/create_codespaces_prebuilds/badge.svg?branch=main)](https://github.com/nogibjj/aws-template/actions/workflows/codespaces/create_codespaces_prebuilds)

## Serverless Data Engineering Pipeline using Hugging Face Transformers library for sentiment analysis

This project reproduced the architecture of the example serverless data engineering project using AWS Lambda for processing, AWS S3 for storage, and AWS Glue for ETL operations. This pipeline will extend the functionality of NLP analysis by allowing us to process and analyze large amounts of text data in a scalable and cost-effective manner.

## Week 9: Run a Serverless "Hello, World!" with AWS Lambda

Created a Hello World Lambda function using the AWS Lambda console. and manually invoke the Lambda function using sample event data and review output metrics.

## Week 10: Setting up AWS Glue

Create a Glue crawler to infer the schema of input data and store it in the Glue Data Catalog. Create a Glue job to perform ETL operations.

## Week 11: schedule and monitor the pipeline

Using AWS CloudWatch Events to schedule pipeline to run at specific intervals, or trigger it based on specific events (e.g., when new data is uploaded to the input S3 bucket).

Monitoring the pipeline using AWS CloudWatch to ensure it's running smoothly and efficiently.

### Used in Following Projects

* [coursera-mlops-aws-c3-step-functions](https://github.com/nogibjj/coursera-mlops-aws-c3-step-functions)
* [coursera-mlops-aws-c3-eda](https://github.com/nogibjj/coursera-mlops-aws-c3-eda)
* [coursera-mlops-aws-c3-linear-regression](https://github.com/nogibjj/coursera-mlops-aws-c3-linear-regression)
* [coursera-mlops-aws-c3-fine-tune-sagemaker-studio-lab](https://github.com/nogibjj/coursera-mlops-aws-c30fine-tune-sagemaker-studio-lab)

### References

* [Watch GitHub Universe Talk:  Teaching MLOps at scale with Github](https://watch.githubuniverse.com/on-demand/ec17cbb3-0a89-4764-90a5-9debb58515f8)
* [Building Cloud Computing Solutions at Scale Specialization](https://www.coursera.org/specializations/building-cloud-computing-solutions-at-scale)
* [Python, Bash and SQL Essentials for Data Engineering Specialization](https://www.coursera.org/learn/web-app-command-line-tools-for-data-engineering-duke)
* [Implementing MLOps in the Enterprise](https://learning.oreilly.com/library/view/implementing-mlops-in/9781098136574/)
* [Practical MLOps: Operationalizing Machine Learning Models](https://www.amazon.com/Practical-MLOps-Operationalizing-Machine-Learning/dp/1098103017)
* [Coursera-Dockerfile](https://gist.github.com/noahgift/82a34d56f0a8f347865baaa685d5e98d)
