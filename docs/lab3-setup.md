# Lab 3: Serverless Data Processing Pipeline

## Architecture Overview
This pipeline automatically processes CSV files uploaded to S3 using serverless AWS services.

## Services Used
- **S3**: File storage and event triggers
- **Lambda**: Data processing logic
- **DynamoDB**: Processed data storage
- **SQS**: Error handling and retry mechanism
- **CloudWatch**: Monitoring and logging

## S3 Bucket Structure
- `raw-data/`: Incoming CSV files
- `processed-data/`: Successfully processed files  
- `failed-data/`: Files that failed processing
- `archive/`: Backup copies

## Sample Data Types
1. Customer orders (e-commerce scenario)
2. Sales transactions (retail scenario)  
3. IoT sensor data (manufacturing scenario)

## Success Metrics
- [ ] Files automatically detected when uploaded
- [ ] CSV data parsed and validated
- [ ] Clean data stored in DynamoDB
- [ ] Failed files handled gracefully
- [ ] Processing monitored with CloudWatch