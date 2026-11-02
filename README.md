# secbyte-digital-forensics-disk-imaging-devsecops-pipeline-security-ctf-labs
A practical collection of cybersecurity CTF labs covering digital evidence handling (disk imaging deep dives, file recovery carving, timeline analysis, chain of custody verification) and DevSecOps security (pipeline hardening, infrastructure-as-code scanning, HashiCorp Vault secret management, container runtime escape detection).
# Digital Forensics, Disk Imaging, Chain of Custody & DevSecOps Pipeline Security CTF Labs

Welcome to the **Digital Forensics, Disk Imaging, Chain of Custody & DevSecOps Pipeline Security CTF Lab Collection**. This repository serves as an organized, searchable catalog of practical cybersecurity labs hosted on Learn SecByte.

This collection focuses on forensically sound evidence collection methodologies, host disk carving, CI/CD pipeline defense, and cloud-native DevSecOps—spanning **Digital Evidence Acquisition & Forensic Integrity (Acquisition-to-courtroom workflows, evidence collection fundamentals, chain of custody verification, disk imaging deep dive)**, **File Recovery & Timeline Analysis (File carving unallocated space, audit trail recovery, chronological event sequencing)**, **DevSecOps Pipeline Hardening & IaC Security (Automated pipeline defense, commit-to-deploy security gates, Terraform/CloudFormation IaC scanning)**, and **Secrets Management & Container Runtime Defense (HashiCorp Vault hygiene, API key hygiene, container runtime escape detection)**.

---

## Lab Collection Index

### 1. Digital Evidence Acquisition, Disk Imaging & Chain of Custody
* **Digital Evidence Fundamentals: From Acquisition to Courtroom**  
  *Lab Link:* [https://learn.secbyte.org/ctf/digital-evidence-fundamentals-from-acquisition-to-courtroom](https://learn.secbyte.org/ctf/digital-evidence-fundamentals-from-acquisition-to-courtroom)  
  *Focus:* Mastering the complete forensic lifecycle—from Order of Volatility volatile memory captures to bit-stream disk acquisition, evidence sealing, and courtroom submission.

* **Evidence Collection Fundamentals**  
  *Lab Link:* [https://learn.secbyte.org/ctf/evidence-collection-fundamentals](https://learn.secbyte.org/ctf/evidence-collection-fundamentals)  
  *Focus:* Executing forensically sound physical and logical evidence acquisitions, utilizing hardware write-blockers, verifying SHA-256 hash pairs, and maintaining integrity during triage.

* **Disk Imaging Deep Dive**  
  *Lab Link:* [https://learn.secbyte.org/ctf/disk-imaging-deep-dive](https://learn.secbyte.org/ctf/disk-imaging-deep-dive)  
  *Focus:* Creating raw (`dd`/`raw`), Expert Witness Format (`.E01`), and Advanced Forensic Format (`.AFF`) images; configuring read error retries; and mounting forensic images read-only.

<Image src="image_agent_tag_11789379615474366990" alt="Digital Forensics Identification Image Acquisition Data Recovery Analysis Reporting Process Diagram" caption="Digital Forensics Identification, Acquisition & Analysis Lifecycle" />

---

* **Chain of Custody: Evidence Integrity Lab**  
  *Lab Link:* [https://learn.secbyte.org/ctf/chain-of-custody-evidence-integrity-lab](https://learn.secbyte.org/ctf/chain-of-custody-evidence-integrity-lab)  
  *Focus:* Structuring tamper-evident evidence tracking ledgers, auditing custody handoff logs, detecting evidence tampering via hash verification failures, and maintaining legally defensible evidence lockers.

* **Evidence Preservation: Chain of Custody Investigation**  
  *Lab Link:* [https://learn.secbyte.org/ctf/evidence-preservation-chain-of-custody-investigation](https://learn.secbyte.org/ctf/evidence-preservation-chain-of-custody-investigation)  
  *Focus:* Investigating evidence handling breaches, identifying gaps in custodial tracking forms, preserving volatile cloud storage snapshots, and maintaining legal admissibility.

### 2. File Recovery Carving & Chronological Timeline Analysis
* **File Recovery Forensics: The Lost Audit Trail**  
  *Lab Link:* [https://learn.secbyte.org/ctf/file-recovery-forensics-the-lost-audit-trail](https://learn.secbyte.org/ctf/file-recovery-forensics-the-lost-audit-trail)  
  *Focus:* Executing file carving operations over unallocated disk space using `photorec`/`scalpel`, parsing raw file headers/footers, and reconstructing deleted security audit logs.

* **Timeline Analysis: The Hidden Sequence**  
  *Lab Link:* [https://learn.secbyte.org/ctf/timeline-analysis-the-hidden-sequence](https://learn.secbyte.org/ctf/timeline-analysis-the-hidden-sequence)  
  *Focus:* Building master forensic timelines (`log2timeline`/`plaso`), correlating MACB file timestamps (Modified, Accessed, Changed, Born), and detecting timestomping anti-forensic techniques.

### 3. DevSecOps Pipeline Hardening & Infrastructure as Code (IaC)
* **DevSecOps Automation: Pipeline Defender**  
  *Lab Link:* [https://learn.secbyte.org/ctf/devsecops-automation-pipeline-defender](https://learn.secbyte.org/ctf/devsecops-automation-pipeline-defender)  
  *Focus:* Embedding automated security testing (SAST/DAST/SCA) into CI/CD build runners (GitHub Actions, GitLab CI), setting security gating thresholds, and breaking non-compliant builds.

<Image src="image_agent_tag_11789379615474367563" alt="DevSecOps infinity loop diagram illustrating integration of security across Plan, Code, Build, Test, Release, Deploy, Operate, and Monitor stages" caption="DevSecOps Continuous Integration & Security Lifecycle" />

---

* **Pipeline Hardening: From Commit to Deploy**  
  *Lab Link:* [https://learn.secbyte.org/ctf/pipeline-hardening-from-commit-to-deploy](https://learn.secbyte.org/ctf/pipeline-hardening-from-commit-to-deploy)  
  *Focus:* Securing build agent environments, enforcing signed Git commits (GPG), preventing unauthorized build pipeline modifications, and auditing deployment service principal roles.

* **Infrastructure as Code Security: Broken Pipeline & Hidden Secrets**  
  *Lab Link:* [https://learn.secbyte.org/ctf/infrastructure-as-code-security-broken-pipeline-hidden-secre](https://learn.secbyte.org/ctf/infrastructure-as-code-security-broken-pipeline-hidden-secre)  
  *Focus:* Scanning Terraform, CloudFormation, and Ansible manifests using Checkov/tfsec; detecting hardcoded API keys and unencrypted storage buckets; and fixing IaC security misconfigurations.

### 4. Secrets Management & Container Security
* **Secret Management: Keys, Tokens, and Vault Hygiene**  
  *Lab Link:* [https://learn.secbyte.org/ctf/secret-management-keys-tokens-vault-hygiene](https://learn.secbyte.org/ctf/secret-management-keys-tokens-vault-hygiene)  
  *Focus:* Implementing HashiCorp Vault dynamic secrets, auditing secret rotation lifecycle policies, purging exposed tokens from Git commit histories (`trufflehog`), and managing API key hygiene.

* **Container Security: From Runtime Basics to Escape Detection**  
  *Lab Link:* [https://learn.secbyte.org/ctf/container-security-from-runtime-basics-to-escape-detection](https://learn.secbyte.org/ctf/container-security-from-runtime-basics-to-escape-detection)  
  *Focus:* Auditing container image vulnerabilities (Trivy/Clair), enforcing AppArmor/seccomp profiles, analyzing runtime container behavior, and detecting host kernel escape attempts.

---

## Learning Path

### Path A: Digital Forensics & Evidence Integrity Specialist
1. **Acquisition & Chain of Custody:** Start with [Digital Evidence Fundamentals](https://learn.secbyte.org/ctf/digital-evidence-fundamentals-from-acquisition-to-courtroom), [Evidence Collection Fundamentals](https://learn.secbyte.org/ctf/evidence-collection-fundamentals), and [Chain of Custody Lab](https://learn.secbyte.org/ctf/chain-of-custody-evidence-integrity-lab).
2. **Imaging & Preservation:** Master disk captures in [Disk Imaging Deep Dive](https://learn.secbyte.org/ctf/disk-imaging-deep-dive) and [Evidence Preservation](https://learn.secbyte.org/ctf/evidence-preservation-chain-of-custody-investigation).

### Path B: File Recovery & Forensic Timeline Analyst
1. **Carving & Log Recovery:** Extract lost artifacts via [File Recovery Forensics](https://learn.secbyte.org/ctf/file-recovery-forensics-the-lost-audit-trail).
2. **Event Sequencing:** Build master timelines using [Timeline Analysis: The Hidden Sequence](https://learn.secbyte.org/ctf/timeline-analysis-the-hidden-sequence).

### Path C: DevSecOps Engineer & Container Security Specialist
1. **Pipeline & IaC Defense:** Hardened automated workflows via [DevSecOps Automation](https://learn.secbyte.org/ctf/devsecops-automation-pipeline-defender), [Pipeline Hardening](https://learn.secbyte.org/ctf/pipeline-hardening-from-commit-to-deploy), and [Infrastructure as Code Security](https://learn.secbyte.org/ctf/infrastructure-as-code-security-broken-pipeline-hidden-secre).
2. **Secrets & Container Runtime:** Audit secrets and workloads in [Secret Management](https://learn.secbyte.org/ctf/secret-management-keys-tokens-vault-hygiene) and [Container Security](https://learn.secbyte.org/ctf/container-security-from-runtime-basics-to-escape-detection).

---

## How to Use the Labs

1. Select a practice scenario from the **Lab Collection Index**.
2. Click the direct link to launch the exercise environment hosted on Learn SecByte.
3. Review scenario directives, raw disk images (`.dd`/`.E01`), GitHub workflow files (`.github/workflows`), Terraform scripts, or container runtime logs.
4. Mount forensic images with write-blockers, carve deleted log files, configure SAST scanning gates in pipeline runners, rotate Vault dynamic tokens, or isolate container escapes to capture flags.

---

## Target Audience

* **Digital Forensic Examiners & Incident Responders:** Acquire bit-stream disk images, maintain chain of custody documentation, carve deleted file artifacts, and construct MACB timelines.
* **DevSecOps & Cloud Security Engineers:** Embed automated SAST/SCA security gates into CI/CD pipelines, scan IaC code templates, and harden secret storage in HashiCorp Vault.
* **Container & Infrastructure Security Analysts:** Audit container base images, enforce seccomp/AppArmor isolation profiles, and detect host container escape vectors.
* **Cybersecurity Students:** Acquire practical hands-on experience in forensically sound evidence handling, CI/CD pipeline protection, and modern cloud security operations.

---

## Disclaimer

All lab links provided in this repository direct to official training environments hosted on Learn SecByte. All materials and exercises are provided strictly for educational purposes, defensive skill building, and authorized security research. Unauthorized forensic acquisition or automated scanning against unauthorized external systems is strictly prohibited.
