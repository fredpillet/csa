# 🧭 Velyo — Connected Sportswear Analytics Platform

Welcome to the Velyo project repository. Velyo is Decathlon’s next-generation analytics backend for connected outdoor sportswear. This project powers secure telemetry collection, transformation, and reporting across thousands of IoT-enabled garments.

> ⚠️ This system processes **sensitive personal activity data**. Security, privacy, and compliance are critical.

---

## 📦 Project Structure

```bash
.
├── infra/                  # Infrastructure as Code (Terraform / Helm)
│   ├── s3.tf               # Secure telemetry storage
│   ├── iam.tf              # Least privilege role definitions
│   └── k8s/                # Kubernetes manifests
├── services/
│   ├── analytics-processor/
│   │   ├── Dockerfile      # Containerized backend processor
│   │   ├── app.py
│   │   └── requirements.txt
├── serverless/
│   └── ingest-handler/     # AWS Lambda for secure data intake
├── scripts/
├── .sentinelone/           # Rego policies & config for SentinelOne
├── .github/                # CI/CD workflows
└── README.md
