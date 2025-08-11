# uptime-unicorn

Curriculum and trackerrr :)

## Week 1 — Linux & AI Foundations
- [/] Linux process commands: ps, top, htop, kill, pkill
- [ ] Networking commands: netstat, ss, curl, dig, nslookup
- [ ] Practice incident triage on CPU/mem/network issues
- [ ] Terraform basics: deploy & destroy AWS EC2
- [ ] Deploy Hugging Face model API locally with FastAPI + Docker
- [ ] Understand ML lifecycle stages (data → deploy → monitor)
- [ ] Networking deep dive: TCP handshake, HTTP vs HTTPS, DNS flow
- [ ] On-call simulation #1: debug API slowness & network outages

## Week 2 — Kubernetes, AI Deployment Basics & GCP Intro
- [ ] Docker basics: run, exec, logs, build images
- [ ] Kubernetes basics: kubectl, minikube, deploy & expose Nginx
- [ ] Compare MLOps tools: MLflow, SageMaker, Vertex AI, Kubeflow
- [ ] Containerize Hugging Face FastAPI app
- [ ] Deploy AI API to Kubernetes with Deployment + Service
- [ ] Install Prometheus + Grafana in minikube
- [ ] Add Prometheus metrics to AI API
- [ ] **GCP Intro**: create GCP project, enable GKE API, deploy Nginx to GKE
- [ ] On-call simulation #2: investigate AI API latency spike, add autoscaling

## Week 3 — Event-Driven Payments, IaC (AWS & GCP), Ansible
- [ ] Terraform stack: AWS VPC, subnets, NAT, security groups, EKS, RDS, S3, IAM
- [ ] Terraform stack (GCP): VPC, GKE cluster, Cloud SQL
- [ ] Kafka topics: payments.raw, payments.enriched, fraud.scores, alerts.incidents
- [ ] Payments Ingest API (FastAPI or Go)
- [ ] Baseline SLIs/SLOs for API
- [ ] Grafana dashboard JSON committed
- [ ] RUNBOOK.md + SLOs.yaml
- [ ] **Ansible**: automate VM setup for Postgres replica or jump host
- [ ] Multi-cloud networking check: connect AWS and GCP services

## Week 4 — Real-Time Enrichment, Model Serving & Multi-Cloud CI/CD
- [ ] Feature Enricher service (Kafka consumer → Kafka producer)
- [ ] Fraud model API on K8s with HPA
- [ ] Scoring Worker service
- [ ] JSON structured logging to Loki/ELK
- [ ] Distributed tracing with OpenTelemetry
- [ ] Load test (k6/Locust) report
- [ ] **CI/CD**: Jenkins or GitHub Actions pipeline for multi-cloud deploy
- [ ] Deploy scoring service to both AWS (EKS) and GCP (GKE) with pipeline toggle

## Week 5 — Data Pipelines, Batch Inference & Cost Controls
- [ ] Airflow DAG for nightly batch inference
- [ ] Lightweight feature store (S3 + Parquet)
- [ ] Redis caching for repeated inference calls
- [ ] Node group right-sizing (spot/ondemand)
- [ ] Cost dashboard / report (AWS + GCP)
- [ ] Error budget policy doc

## Week 6 — Reliability Hardening, Chaos & DR
- [ ] Chaos tests: kill model API, drop Kafka broker, simulate DB failover
- [ ] DR playbook with RTO/RPO targets
- [ ] Symptom-based alert tuning
- [ ] Rate limiting & bulkheads at API ingress
- [ ] Two fictional but realistic postmortems

## Week 7 — Security, Compliance & Data/Model Governance
- [ ] mTLS in cluster, TLS at edge, secrets in KMS
- [ ] Image signing (Cosign), OPA policies
- [ ] PII tokenization/encryption
- [ ] Model registry with versioning + signed artifacts
- [ ] Audit trail for infra/model changes
- [ ] Threat model diagram

## Week 8 — Polish, Performance & Interview Readiness
- [ ] k6 performance tests with results
- [ ] Local mini-stack demo (Kind + localstack + Redpanda)
- [ ] Context/container/dataflow diagrams
- [ ] Two deep-dive writeups (SRE + AI angle)
- [ ] STAR bullets for behavioral
- [ ] Public/sanitized GitHub repo with docs & diagrams

