# Aqua Security is the home of Trivy

[Trivy](https://github.com/aquasecurity/trivy), the industry's leading open source security scanner is proudly maintained by Aqua Security. If you like Trivy, you will love Aqua, which builds on top of Trivy to provide even more enhanced capabilities for a complete security management offering.

## User experience

| Feature | Trivy OSS | Aqua |
| --- | --- | --- |
| Interface | CLI tool | CLI tool <br> Enterprise-grade web application <br> SaaS or on-prem |
| Search & Discover | - | Easily search for security issues across all workloads and infrastructure in your organization <br> Visually discover risks across your organization |
| User management | - | Multi account <br> Granular permissions (RBAC) <br> Single Sign On (SSO) |
| Support | Some skills required for setup and integration <br> Best effort community support | Personal onboarding by Aqua Customer SuccessSLA backed professional support |
| Scalability & Availability | Single scan at a time
 | Centralized scanning service supports concurrent scans efficiently <br> Highly available production grade architecture |

## Vulnerability scanning

| Feature | Trivy OSS | Aqua |
| --- | --- | --- |
| Vulnerabilities sources | Based on open source vulnerability feeds | Based on open source and commercial vulnerability feeds |
| New Vulnerabilities SLA | No SLA | Commercial level SLA |
| Vulnerability management | Manually ignore specific vulnerabilities by ID or property | Advanced vulnerability management solution <br> Vulnerability tracking and suppression <br> Incident lifecycle management |
| Vulnerability prioritization | Manually triage by severity
 | Multiple prioritization tools:  <br> Accessibility of the affected resources <br> Exploitability of the vulnerability <br> Open Source packages health and trustworthiness score <br> Affected image layers |
| Contextual vulnerabilities | - | Reduce irrelevant vulnerabilities based on environmental factors (e.g. Spring4Shell not relevant due to JDK version) |
| Compiled binaries | Find embedded dependencies in Go, Rust binaries <br> Find SBOM by hash in public Sigstore | In addition to identifying binary by hash, identifies popular applications by flexible heuristics |

## Container scanning

| Feature | Trivy OSS | Aqua |
| --- | --- | --- |
| Windows containers | - | Support scanning windows containers |
| Scan container registries | - | Connect to any container registries and automatically scan it |
| Private registries | Standard registry authenticationCloud authentication with ECR, GCR, ACR | Supports different registry specific authentication schemes |
| Layer cache | Local cache directory | Scalable Cloud cache |

## Advanced scanning

| Feature | Trivy OSS | Aqua |
| --- | --- | --- |
| Malware scanning | - | Scan container images for malware |
| Sandbox scanning | - | Use DTA (Dynamic threat analysis) to run and test container images' behavior to detect sophisticated threats |

## Policy and enforcement

| Feature | Trivy OSS | Aqua |
| --- | --- | --- |
| Kubernetes admission | - | Validating Kubernetes Admission based on automatic or user defined policy |
| Container engine | - | Block incompliant images from running at container engine level |
| Block vulnerable packages | - | vShield – monitor and block usage of vulnerable packages |

## Secrets scanning

| Feature | Trivy OSS | Aqua |
| --- | --- | --- |
| Detected patterns | Basic patterns | Advanced patterns |
| Leaked secrets validation | - | Automatically checks if leaked secrets are valid and usable |

## IaC/CSPM scanning

| Feature | Trivy OSS | Aqua |
| --- | --- | --- |
| Infrastructure as Code (IaC) | Many popular languages as detailed [here](../docs/scanner/misconfiguration/policy/builtin.md) | Same as Trivy |
| Checks customization | Create custom checks with Rego | Create custom checks in no-code interface <br> Customize existing checks with organizational preferences |
| Cloud scanning | AWS, Azure, GCP | AWS, Azure, GCP, Alibaba Cloud, Oracle Cloud |
| Compliance frameworks | CIS, vendor guides | More than 25 compliance programs |
| Custom compliance | Manually in text file | Create your own compliance program through a web application |
| Remediation advice | Basic | AI powered specialized remediation guides |

## Kubernetes scanning

| Feature | Trivy OSS | Aqua |
| --- | --- | --- |
User experience - trigger scan | CLI <br> Automated with Kubernetes Operator | Automated with Kubernetes Operator </br> Advanced UI web application |
User experience - consume results | kubectl/CRD <br> Prometheus exporter | kubectl/CRD <br> Advanced UI dashboards <br> Automatic notifications and incident management |
Cluster discovery | Kubectl/Kubeconfig | Automatic discovery thorough cloud |
Workload image scanning | Scanning in cluster, requires capacity planning | Scanning offloaded to Aqua service, little impact on scanned clusters |
| Cluster scanning | CIS, NSA, PSS | More than 25 compliance programs |
| Scope |  Single cluster | Multi cluster, Cloud relationship |
| Scalability | Reports limited by in-cluster storage (size and number of reports) | Cloud-based storage (unlimited scalability) |
