# Policy as Code (PaC) Templates Collection

This repository contains a comprehensive collection of Policy as Code (PaC) artifacts from various open source PaC libraries. It serves as a reference for different policy frameworks, patterns, and implementations across various platforms and technologies.

## Project Structure

The repository is organized into three main categories:

### 1. Infrastructure

Contains policies for infrastructure management and cloud security:

- **OPA**: Open Policy Agent policies for cloud providers
  - AWS (acm, api-gw, cloudfront, cloudtrail, etc.)
  - Azure (app-gateway, cognitive-services, cosmos-db, etc.)
  
- **Sentinel**: HashiCorp Sentinel policies for Terraform
  - Includes policies for cost management, resource restrictions, provider constraints, etc.

### 2. Kubernetes

Kubernetes-focused policies for cluster security and configuration:

- **OPA-Gatekeeper**: Policies implemented as Gatekeeper constraints
  - General policies (allowed repositories, container limits, ingress controls, etc.)
  - Pod Security Policies (privilege controls, host access restrictions, etc.)

- **Kyverno**: Extensive collection of Kyverno policies
  - Best practices
  - Pod security standards
  - Integration with tools (Argo, AWS, Istio, Flux, etc.)
  - Platform-specific policies (OpenShift, etc.)

### 3. Application

Application and container-level policies:

- Configuration specific policies
  - Version requirements
  - Package scope controls
  - Publishing configuration checks

- Container-image-specific policies
  - Registry restrictions
  - Secret and sensitive data management

## Statistics

This repository contains a total of **1,688 policy files** across all categories:

| Category | File Count |
|----------|------------|
| Infrastructure | 293 |
| Kubernetes | 1,385 |
| Application | 10 |

### Policy Types Breakdown

| Policy Type | File Count |
|-------------|------------|
| YAML policies (Kyverno, etc.) | 1,379 |
| Rego policies (OPA) | 109 |
| HCL policies (Sentinel) | 77 |
| Other policy formats | 123 |

## Purpose

This collection serves multiple purposes:

- **Reference Implementation**: Provides practical examples of policies for various platforms
- **Learning Resource**: Helps users understand different policy frameworks and their syntax
- **Policy Library**: Can be used as a starting point for implementing your own policies
- **Best Practices**: Demonstrates recommended security and governance approaches

## Contributing

Contributions to this policy collection are welcome. Please feel free to submit a pull request with new policies or improvements to existing ones.

## License

Please check the license of individual policies as they may have been sourced from different open source projects. 