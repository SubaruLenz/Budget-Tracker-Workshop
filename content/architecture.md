---
title: "AWS Architecture"
description: "Cloud-native architecture with AWS services"
showTableOfContents: true
---

## Architecture Overview

![AWS Architecture](logo.png)

Our cloud-native budget tracker leverages multiple AWS services to provide a scalable, secure, and intelligent financial management solution.

## Compute Layer

### Amazon ECS Fargate
- **Serverless container hosting** for the FastAPI backend
- **Auto-scaling** based on demand
- **No server management** required

### Application Load Balancer
- **Traffic distribution** across multiple containers
- **SSL termination** for secure connections
- **Health checks** for container monitoring

## Database Architecture

### Amazon Aurora PostgreSQL
- **Primary database** with read replicas for performance
- **Automated backups** with point-in-time recovery
- **Connection pooling** for optimized database connections
- **VPC endpoints** for secure database access

## AI Integration

### AWS Bedrock
- **Foundation Models**: Claude, Titan, or Jurassic models for financial advice
- **Conversation Management**: Persistent chat sessions with context
- **Financial Analysis**: AI-powered spending pattern recognition
- **Security**: IAM roles for secure Bedrock API access

## Security & Networking

### Amazon VPC
- **Private subnets** with NAT Gateways
- **Multi-AZ deployment** for high availability
- **Security groups** for network access control

### AWS Secrets Manager
- **Secure credential management**
- **Automatic rotation** of database passwords
- **Integration** with ECS tasks

## Monitoring & Observability

### Amazon CloudWatch
- **Application metrics** and custom dashboards
- **Log aggregation** with CloudWatch Logs
- **Performance monitoring** and alerting
- **Cost tracking** and optimization insights

## Key Benefits

{{< alert "check" >}}
**Scalability** - Auto-scaling based on demand  
**Security** - VPC isolation and encrypted data  
**Cost-Effective** - Pay-per-use serverless model  
**AI-Powered** - Intelligent financial insights  
**High Availability** - Multi-AZ deployment
{{< /alert >}}