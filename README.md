# AWS Architecture Icons Repository

A comprehensive collection of AWS architecture icons organized for easy access and use in technical documentation, presentations, and diagrams.

[![Latest Release](https://img.shields.io/github/v/release/icacho-dev/aws-architecture-icons?style=flat-square)](https://github.com/icacho-dev/aws-architecture-icons/releases)
[![License](https://img.shields.io/github/license/icacho-dev/aws-architecture-icons?style=flat-square)](LICENSE)
[![Issues](https://img.shields.io/github/issues/icacho-dev/aws-architecture-icons?style=flat-square)](https://github.com/icacho-dev/aws-architecture-icons/issues)

## 📋 Table of Contents

- [Overview](#overview)
- [Repository Structure](#repository-structure)
- [Usage Examples](#usage-examples)
- [Icon Categories](#icon-categories)
- [Integration Guide](#integration-guide)
- [File Formats and Sizes](#file-formats-and-sizes)
- [Quick Reference](#quick-reference)
- [Contributing](#contributing)
- [License](#license)

## 🌟 Overview

This repository contains the latest AWS architecture icons (February 2025 release) organized in a clear, accessible structure. Perfect for:

- ✅ Technical documentation
- ✅ Architecture diagrams
- ✅ Presentations and slides
- ✅ Training materials
- ✅ Web applications and dashboards

## 📁 Repository Structure

```
📦 aws-architecture-icons/
├── 🏗️  Architecture-Group-Icons_02072025/     # Structural elements (VPC, subnets, etc.)
├── 🔧  Architecture-Service-Icons_02072025/   # AWS service icons by category
├── 📂  Category-Icons_02072025/              # Category grouping icons
└── 🎯  Resource-Icons_02072025/              # Specific resource icons
```

### Icon Organization

**Architecture Service Icons** are organized by AWS service categories:
- **Analytics** (Athena, QuickSight, Redshift, etc.)
- **Compute** (EC2, Lambda, ECS, etc.)
- **Database** (RDS, DynamoDB, ElastiCache, etc.)
- **Networking & Content Delivery** (CloudFront, VPC, ELB, etc.)
- **Security, Identity & Compliance** (IAM, Cognito, KMS, etc.)
- **Storage** (S3, EBS, EFS, etc.)
- And 18+ more categories

## 🚀 Usage Examples

### Mermaid Diagrams

```mermaid
graph TD
    subgraph Internet
        A[<img src='https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/Resource-Icons_02072025/Res_General-Icons/Res_48_Light/Res_Users_48_Light.svg' width='40px'><br>Users]
    end

    subgraph "AWS Cloud"
        subgraph "VPC"
            CF[<img src='https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/Architecture-Service-Icons_02072025/Arch_Networking-Content-Delivery/48/Arch_Amazon-CloudFront_48.svg' width='40px'><br>CloudFront<br>CDN]
            
            subgraph "Public Subnet"
                ALB[<img src='https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/Architecture-Service-Icons_02072025/Arch_Networking-Content-Delivery/48/Arch_Elastic-Load-Balancing_48.svg' width='40px'><br>Application<br>Load Balancer]
                AGW[<img src='https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/Architecture-Service-Icons_02072025/Arch_Networking-Content-Delivery/48/Arch_Amazon-API-Gateway_48.svg' width='40px'><br>API Gateway]
            end
            
            subgraph "Private Subnet"
                L[<img src='https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/Architecture-Service-Icons_02072025/Arch_Compute/48/Arch_AWS-Lambda_48.svg' width='40px'><br>Lambda<br>Functions]
                EC2[<img src='https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/Architecture-Service-Icons_02072025/Arch_Compute/48/Arch_Amazon-EC2_48.svg' width='40px'><br>EC2<br>Instances]
            end
            
            subgraph "Data Layer"
                DB[<img src='https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/Architecture-Service-Icons_02072025/Arch_Database/48/Arch_Amazon-DynamoDB_48.svg' width='40px'><br>DynamoDB]
                S3[<img src='https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/Architecture-Service-Icons_02072025/Arch_Storage/48/Arch_Amazon-S3_48.svg' width='40px'><br>S3 Bucket<br>Static Assets]
                RDS[<img src='https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/Architecture-Service-Icons_02072025/Arch_Database/48/Arch_Amazon-RDS_48.svg' width='40px'><br>RDS<br>PostgreSQL]
            end
        end
        
        subgraph "Security & Monitoring"
            IAM[<img src='https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/Architecture-Service-Icons_02072025/Arch_Security-Identity-Compliance/48/Arch_AWS-Identity-and-Access-Management_48.svg' width='40px'><br>IAM<br>Roles & Policies]
            CW[<img src='https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/Architecture-Service-Icons_02072025/Arch_Management-Governance/48/Arch_Amazon-CloudWatch_48.svg' width='40px'><br>CloudWatch<br>Logs & Metrics]
        end
    end

    A --> CF
    CF --> ALB
    ALB --> AGW
    AGW --> L
    L --> DB
    L --> S3
    AGW --> EC2
    EC2 --> RDS
    L -.-> CW
    EC2 -.-> CW
    IAM -.-> L
    IAM -.-> EC2
```

### HTML/Markdown

```html
<!-- Direct usage in HTML -->
<img src="https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/Architecture-Service-Icons_02072025/Arch_Compute/48/Arch_AWS-Lambda_48.svg" width="48" alt="AWS Lambda">

<!-- In Markdown -->
![AWS Lambda](https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/Architecture-Service-Icons_02072025/Arch_Compute/48/Arch_AWS-Lambda_48.svg)
```

### Draw.io / Lucidchart

1. Download the SVG files locally
2. Import as custom shapes/stencils
3. Use in your diagrams

## 🏷️ Icon Categories

### Architecture Service Icons (24 Categories)
| Category | Examples | Count |
|----------|----------|-------|
| **Analytics** | Athena, QuickSight, Redshift | 15+ |
| **Compute** | EC2, Lambda, ECS, Fargate | 20+ |
| **Database** | RDS, DynamoDB, Aurora | 12+ |
| **Networking** | VPC, CloudFront, Route 53 | 18+ |
| **Security** | IAM, Cognito, KMS, WAF | 15+ |
| **Storage** | S3, EBS, EFS, Glacier | 10+ |
| **AI/ML** | SageMaker, Rekognition, Lex | 12+ |
| **Containers** | EKS, ECS, ECR | 8+ |

[View all categories →](Architecture-Service-Icons_02072025/)

### Resource Icons
Specific resource representations for detailed architecture diagrams.

### Group Icons
Structural elements like VPCs, subnets, availability zones, and regions.

## 🔧 Integration Guide

### CDN URLs
All icons are available via GitHub's raw content URLs:

```
https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/{path-to-icon}
```

### Local Development
```bash
# Clone the repository
git clone https://github.com/icacho-dev/aws-architecture-icons.git

# Use icons locally
cd aws-architecture-icons
```

### Popular Tools Integration

**Mermaid.js**: Use raw GitHub URLs in `<img>` tags  
**Draw.io**: Import SVG files as custom libraries  
**Lucidchart**: Upload SVG files as custom shapes  
**PowerPoint**: Copy and paste SVG files directly  
**Figma**: Import SVG files as components

## 📏 File Formats and Sizes

### Available Formats
- **SVG**: Vector format, scalable, recommended for web
- **PNG**: Raster format, good for presentations

### Available Sizes
- **16px**: Small icons for compact layouts
- **32px**: Medium icons for standard use
- **48px**: Large icons for prominent display
- **64px**: Extra large icons for presentations

### File Naming Convention
```
{Type}_{Service-Name}_{Size}.{format}
```

Examples:
- `Arch_AWS-Lambda_48.svg`
- `Res_Amazon-S3_32.png`

## ⚡ Quick Reference

### Most Popular Icons

| Service | 48px SVG Link |
|---------|---------------|
| **Lambda** | [📎 SVG](https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/Architecture-Service-Icons_02072025/Arch_Compute/48/Arch_AWS-Lambda_48.svg) |
| **S3** | [📎 SVG](https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/Architecture-Service-Icons_02072025/Arch_Storage/48/Arch_Amazon-S3_48.svg) |
| **EC2** | [📎 SVG](https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/Architecture-Service-Icons_02072025/Arch_Compute/48/Arch_Amazon-EC2_48.svg) |
| **RDS** | [📎 SVG](https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/Architecture-Service-Icons_02072025/Arch_Database/48/Arch_Amazon-RDS_48.svg) |
| **API Gateway** | [📎 SVG](https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/Architecture-Service-Icons_02072025/Arch_Networking-Content-Delivery/48/Arch_Amazon-API-Gateway_48.svg) |

### URL Template
```
https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/
Architecture-Service-Icons_02072025/
Arch_{Category}/
{Size}/
Arch_{Service-Name}_{Size}.svg
```

## 🤝 Contributing

We welcome contributions! Please:

1. 🍴 Fork the repository
2. 🔄 Create a feature branch
3. 📝 Submit a pull request

### Reporting Issues
Found a missing icon or broken link? [Open an issue](https://github.com/icacho-dev/aws-architecture-icons/issues/new).

## 📄 License

Icons are sourced from AWS and organized for community use. Please refer to [AWS's official icon usage guidelines](https://aws.amazon.com/architecture/icons/) for commercial usage terms.

---

## 💡 Tips & Best Practices

- **Use SVG format** for web applications and scalable diagrams
- **Use 48px size** for most documentation needs
- **Combine with group icons** for complete architecture diagrams
- **Cache locally** for offline presentations
- **Maintain consistency** in icon sizes within the same diagram

> **Note**: This repository is updated regularly with the latest AWS icon releases. Star ⭐ the repo to stay updated!
