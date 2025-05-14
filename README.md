[![CI](https://github.com/nogibjj/aws-template/actions/workflows/cicd.yml/badge.svg?branch=main)](https://github.com/nogibjj/aws-template/actions/workflows/cicd.yml)
[![Codespaces Prebuilds](https://github.com/nogibjj/aws-template/actions/workflows/codespaces/create_codespaces_prebuilds/badge.svg?branch=main)](https://github.com/nogibjj/aws-template/actions/workflows/codespaces/create_codespaces_prebuilds)

# Serverless Data Engineering Pipeline via AWS and Hugging Face Transformers library for sentiment analysis

This project demonstrates a serverless data engineering pipeline that processes and analyzes text data using AWS services and the Hugging Face Transformers library. The pipeline is designed to be scalable, cost-effective, and easy to maintain.

## Architecture

```
┌─────────────┐     ┌─────────────┐     ┌─────────────┐
│  Input S3   │────▶│   Lambda    │────▶│  Output S3  │
│   Bucket    │     │  Function   │     │   Bucket    │
└─────────────┘     └──────┬──────┘     └─────────────┘
                           │
                           ▼
                    ┌─────────────┐
                    │    Glue     │
                    │  (ETL/ETL)  │
                    └──────┬──────┘
                           │
                           ▼
                    ┌─────────────┐
                    │ CloudWatch  │
                    │  (Monitor)  │
                    └─────────────┘
```

## Key Components

### 1. AWS Lambda

- Serverless function for text processing
- Integrates with Hugging Face for sentiment analysis
- Triggered by new data uploads

### 2. AWS S3

- Input bucket for raw text data
- Output bucket for processed results
- Secure and scalable storage

### 3. AWS Glue

- ETL operations
- Schema inference
- Data catalog management

### 4. AWS CloudWatch

- Pipeline monitoring
- Scheduled executions
- Performance metrics

## Getting Started

1. **Prerequisites**

   - AWS Account
   - Python 3.8+
   - AWS CLI configured

2. **Installation**

   ```bash
   pip install -r requirements.txt
   ```

3. **Configuration**

   - Set up AWS credentials
   - Configure S3 buckets
   - Deploy Lambda function

4. **Running the Pipeline**
   ```bash
   python main.py
   ```

## Project Structure

```
.
├── lambda_function.py    # AWS Lambda handler
├── main.py              # Main pipeline script
├── requirements.txt     # Python dependencies
├── tf-requirements.txt  # Terraform dependencies
└── utils/              # Utility functions
```

## Related Projects

- [MLOps AWS Step Functions](https://github.com/nogibjj/coursera-mlops-aws-c3-step-functions)
- [MLOps AWS EDA](https://github.com/nogibjj/coursera-mlops-aws-c3-eda)
- [MLOps AWS Linear Regression](https://github.com/nogibjj/coursera-mlops-aws-c3-linear-regression)

## Resources

- [Building Cloud Computing Solutions at Scale](https://www.coursera.org/specializations/building-cloud-computing-solutions-at-scale)
- [Python, Bash and SQL for Data Engineering](https://www.coursera.org/learn/web-app-command-line-tools-for-data-engineering-duke)
- [Practical MLOps](https://www.amazon.com/Practical-MLOps-Operationalizing-Machine-Learning/dp/1098103017)

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
