````markdown name=README.md
## Example Architecture Diagram

Below is a sample architecture diagram rendered with [Mermaid](https://mermaid-js.github.io/mermaid/#/) and using icons from this repository:

```mermaid
graph TD
    subgraph Internet
        A[<img src='https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/Resource-Icons_02072025/Res_General-Icons/Res_48_Light/Res_Users_48_Light.svg' width='40px'><br>cURL / Client]
    end

    subgraph AWS Cloud
        AGW[<img src='https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/refs/heads/main/Architecture-Service-Icons_02072025/Arch_Networking-Content-Delivery/48/Arch_Amazon-API-Gateway_48.svg' width='40px'><br>API Gateway<br>Handles GET /greet]

        subgraph Authentication & Authorization
            COGNITO[<img src='https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/Architecture-Service-Icons_02072025/Arch_Security-Identity-Compliance/48/Arch_Amazon-Cognito_48.svg' width='40px'><br>Amazon Cognito<br>User Pools]
        end

        L[<img src='https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/Architecture-Service-Icons_02072025/Arch_Compute/48/Arch_AWS-Lambda_48.svg' width='40px'><br>AWS Lambda<br>NestJS API]
        CW[<img src='https://raw.githubusercontent.com/icacho-dev/aws-architecture-icons/main/Architecture-Service-Icons_02072025/Arch_Management-Governance/48/Arch_Amazon-CloudWatch_48.svg' width='40px'><br>CloudWatch Logs<br>Logs & Metrics]
    end

    A --> AGW
    AGW -- Authenticates with --> COGNITO
    AGW --> L
    L --> CW
```

> **Note:** Mermaid diagrams with embedded images render best on supported platforms. For GitHub, you may need to use a browser extension or render the diagram externally.

---

## About

This project hosts AWS architecture icons for easy use in technical documentation and diagrams.  
Icons are sourced and organized for clarity and convenience.
````