# Security Policy

This repository is an educational documentation project. Do not use public GitHub issues or pull requests to disclose live vulnerabilities, confidential audit findings, customer information, credentials, private vendor reports, or other sensitive evidence.

## Reporting a security concern

- For a vulnerability in a code example or repository configuration, use GitHub's private vulnerability reporting feature if it is enabled for this repository, or contact the repository maintainers through a private channel listed in the repository profile.
- For mistakes in framework summaries, provide the affected file, section, official source, and suggested correction without sharing confidential artifacts.
- If a secret is accidentally committed, revoke or rotate it immediately. Deleting the file in a later commit does not remove it from Git history. Follow your provider's incident-response guidance and clean history only with coordinated maintainer review.

## Safe contribution rules

Use fictional or anonymized data. Never include access tokens, API keys, passwords, private keys, customer exports, full assurance reports, or restricted evidence. The `.gitignore` file excludes common local evidence folders, but it is not a substitute for reviewing `git status` and the diff before committing.
