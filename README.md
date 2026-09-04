# PASTA-Threat-modelling-Sneaker-app
Threat modeling a mobile sneaker shopping application using the PASTA methodology.

# PASTA Threat Modeling — Sneaker Shopping Application

## Overview

This project involved using the **PASTA (Process for Attack Simulation and Threat Analysis)** methodology to perform a threat modeling exercise for a mobile application used by a sneaker company.

The application allows customers to purchase products and process financial transactions, so protecting customer information and securing the application's payment functionality are important security objectives.

The assessment was completed by working through the seven stages of the PASTA methodology.

---

## Business and Security Objectives

The application is designed to:

- Allow customers to purchase products through the mobile application.
- Process financial transactions.
- Protect customer information.
- Adhere to **PCI DSS (Payment Card Industry Data Security Standard)** requirements.

---

## Stage I — Define Business and Security Objectives

The main business and security requirements identified for the application were:

- Product purchasing through the mobile application.
- Processing financial transactions.
- Compliance with PCI DSS.

These requirements help establish the security priorities for the application.

---

## Stage II — Define the Technical Scope

The technologies and components considered in the assessment included:

- Application Programming Interface (API)
- Public Key Infrastructure (PKI)
- SHA-256
- SQL

### API

The API provides a way for different software components and third-party services to communicate and interact.

### PKI

Public Key Infrastructure (PKI) can be used to help secure the exchange of sensitive customer information.

### SHA-256

SHA-256 was considered for protecting sensitive information such as usernames and passwords.

### SQL

SQL is used to interact with customer records stored in the application's database.

---

## Stage III — Decompose the Application

The application was broken down into its major components and data flows.

A sample data flow diagram was used to understand how information moves through the application and identify areas that could require additional security controls.

---

## Stage IV — Threat Analysis

The main threats identified during the assessment were:

### Cross-Site Scripting (XSS)

XSS attacks can occur when an application does not properly handle user-controlled input, potentially allowing malicious scripts to be introduced.

### SQL Injection

SQL injection can occur when user input is improperly handled and allows malicious SQL statements to interact with the application's database.

---

## Stage V — Vulnerability Analysis

The assessment identified two important weaknesses:

- Lack of input sanitization
- Lack of prepared statements

These weaknesses could increase the application's exposure to attacks such as XSS and SQL injection.

---

## Stage VI — Attack Modeling

An attack tree was used to model possible attack paths against the application.

The attack modeling stage helps show how an attacker could potentially move from an initial point of attack toward a security objective.

---

## Stage VII — Risk Analysis and Impact

The final stage focused on security controls that could help reduce the identified risks.

The controls considered included:

- Prepared statements
- Hashing
- Public Key Infrastructure (PKI)
- Principle of least privilege

These controls can help reduce the potential impact of vulnerabilities identified during the earlier stages of the assessment.

---

## Key Takeaways

This project helped me understand how threat modeling can be used before or during application development to identify potential security weaknesses.

Some of my main takeaways were:

- Security should be considered alongside business requirements.
- Understanding an application's architecture helps identify potential attack surfaces.
- Vulnerabilities such as poor input handling can create opportunities for attacks.
- Threat modeling provides a structured way to think about how an application could be attacked.
- Security controls should be considered based on the risks identified during the assessment.

---

## Skills Demonstrated

- Threat Modeling
- PASTA Methodology
- Application Security
- Risk Analysis
- Vulnerability Analysis
- Attack Modeling
- SQL Injection Awareness
- Cross-Site Scripting (XSS)
- API Security Concepts
- PKI Concepts
- Principle of Least Privilege

---

## Project Context

**Project type:** Threat modeling exercise

**Methodology:** PASTA

**Application:** Mobile sneaker shopping application

**Focus:** Application security, threat analysis, vulnerability analysis, and risk assessment

---

## Reflection

This project gave me a better understanding of how security risks can be considered from both a business and technical perspective.

Working through the seven stages of PASTA helped me see how an application can be examined systematically, from defining its objectives and technical scope to identifying threats, vulnerabilities, possible attack paths, and security controls.
