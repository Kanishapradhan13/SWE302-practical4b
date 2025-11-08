# Practical 4b: Setting up DAST with OWASP ZAP in GitHub Actions

## Overview

This practical demonstrates how to integrate Dynamic Application Security Testing (DAST) using OWASP ZAP into a CI/CD pipeline with GitHub Actions. DAST complements SAST by identifying runtime vulnerabilities in running applications, simulating real-world attacks, and providing actionable security insights.

## Objectives

- Understand the fundamentals of DAST and OWASP ZAP
- Set up OWASP ZAP scans in GitHub Actions workflows
- Configure scan rules and interpret security findings
- Generate and analyze ZAP security reports
- Integrate DAST results into the development lifecycle

## Learning Outcomes

By completing this practical, you will be able to:

- Explain the difference between SAST and DAST
- Deploy and test a Spring Boot application for DAST
- Configure and run OWASP ZAP baseline and full scans in CI/CD
- Analyze ZAP reports and map findings to OWASP Top 10
- Create remediation plans for identified vulnerabilities
- Integrate security scanning into automated workflows

## Steps Involved

1. **Introduction to DAST and OWASP ZAP**
	- Explored DAST methodology and OWASP ZAP features

2. **Environment Setup**
	- Verified Java and Maven installations
	- Built and ran the Spring Boot application locally

3. **Application Dockerization**
	- Ensured the presence of a Dockerfile for containerized deployment

4. **GitHub Actions Workflow Configuration**
	- Created `.github/workflows/zap-scan.yml` for automated ZAP scans
	- Configured steps to build, deploy, and scan the application

5. **ZAP Rules Configuration**
	- Created `.zap/rules.tsv` to customize scan thresholds and actions

6. **Running ZAP Scans**
	- Executed baseline and full scans via GitHub Actions
	- Generated HTML and JSON reports as workflow artifacts

7. **Security Findings Analysis**
	- Reviewed ZAP reports and identified vulnerabilities
	- Mapped findings to OWASP Top 10 categories
	- Developed a remediation roadmap

8. **Integration with GitHub Security**
	- (Optional) Converted ZAP results to SARIF and uploaded to GitHub Security tab

## Conclusions

- DAST with OWASP ZAP provides essential runtime security coverage, complementing SAST tools like SonarCloud.
- Integrating ZAP into GitHub Actions enables automated, continuous security testing for every code change.
- Regular scanning and analysis help identify and remediate vulnerabilities before production deployment.
- Custom rules and advanced configuration allow for tailored security policies and reduced false positives.
- Combining SAST and DAST in the CI/CD pipeline ensures comprehensive application security.

