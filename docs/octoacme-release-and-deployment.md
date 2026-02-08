# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans (Security Lead sign-off)
- Release notes drafted
- Rollback / mitigation plan documented (DevOps Engineer)
- Smoke tests prepared
- Customer-facing documentation updated (with Customer Success input)

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred, managed by DevOps)
- [ ] Run post-deploy verifications
- [ ] Security validation post-deployment
- [ ] Announce release to stakeholders and support
- [ ] Customer Success team briefed on new features/changes

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call (DevOps Engineer leads)
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items
  - Notify Customer Success if customer-impacting

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
