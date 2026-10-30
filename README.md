Information Security System 🔐📊
A comprehensive repository documenting core information security exercises, enterprise vulnerability assessments, network intrusion detection setup, directory services configuration, cryptographic implementation, and digital integrity checks.

📋 Table of Contents
Overview

Vulnerability Assessment & Management

Directory Services & Authentication (LDAP & Kerberos)

Intrusion Detection Systems (Snort IDS)

Cryptographic Mechanisms & Integrity Verification

🔎 Overview
This lab project explores foundational security engineering and defensive operations, highlighting automated vulnerability scanning, secure enterprise authentication models, packet-level intrusion detection, and cryptographic file protection.

🛡️ Vulnerability Assessment & Management
Nessus Scanning: Conducted comprehensive host and network vulnerability scans (e.g., Windows 7 asset scans) to identify missing patches, security misconfigurations, and software end-of-life vulnerabilities.

Report Analysis: Analyzed risk vectors, categorized findings by severity, and prioritized remediation actions.

🗂️ Directory Services & Authentication (LDAP & Kerberos)
OpenLDAP Implementation: Configured master LDAP servers (ldap.example.com) and client systems using slapd, provisioning organizational units (ou=demo), user schemas (inetOrgPerson, posixAccount), and secure password hashing (SSHA).

Kerberos Realm Configuration: Set up a fully functional Kerberos V5 authentication server (krbsrv.example.com) and workstation client (krbclient.example.com), managing principals, keytabs (/etc/krb5.keytab), and ticket generation (kinit, klist) for secure remote shell access via SSH.

🚨 Intrusion Detection Systems (Snort IDS)
Snort Configuration: Deployed and configured Snort IDS on Ubuntu virtual interfaces (enp0s8 in promiscuous mode) to monitor network traffic.

Custom Rule Writing: Developed custom organizational detection rules (ORG.rules) to capture specific malicious or anomalous traffic patterns, such as ICMP echo requests and unauthorized SSH connection attempts.

🔑 Cryptographic Mechanisms & Integrity Verification
Asymmetric Signatures: Generated RSA private/public key pairs using openssl to sign confidential documents and verify data integrity and non-repudiation (Verified OK vs. Verification Failure upon content tampering.

Symmetric Encryption: Implemented command-line and desktop file encryption using AES Crypt to secure sensitive media assets (.aes).

Message Digest Integrity: Validated file integrity across state changes using checksum algorithms (md5sum).
