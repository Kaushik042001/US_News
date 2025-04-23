# 🏗️ GCP Column-Level Access Control using Terraform

This Terraform project is designed to implement **column-level security** and **fine-grained access control** across GCP services such as **BigQuery**, **Data Catalog**, and **GCS**, with policy-driven role management for **analysts**, **developers**, and **admins**.

---

## 📂 Project Structure

```plaintext
.
├── backend.tf
├── main.tf
├── provider.tf
├── terraform.tfvars
├── variables.tf
├── env/                  # Environment-specific tfvars
├── modules/              # Reusable Terraform modules
│   ├── bigquery/
│   ├── data_catalog/
│   ├── dlp/
│   ├── gcs/
│   └── iam/
│       ├── policy_bindings/
│       ├── policy_tag_binding/
│       └── roles/
├── bootstrap/            # Bootstrap Terraform configs
├── scripts/              # Automation scripts
│   └── apply_policy_tags.py
├── config/
│   ├── policy_tags_mapping.yaml
│   └── terraform_outputs.json
└── service_accounts/     # GCP service account keys
