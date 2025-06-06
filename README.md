# MERN Stack App with GitHub Actions CI/CD

## 📋 Description

This is a full-stack MERN (MongoDB, Express.js, React, Node.js) application configured with a CI/CD pipeline using **GitHub Actions**. It runs **Cypress component tests** automatically when a Pull Request is made to the `develop` branch, and **deploys to Render** when code is merged into the `main` branch.

## 🚀 Features

- Full-stack MERN architecture
- Cypress component testing
- GitHub Actions integration for CI/CD
- Deployment to [Render](https://render.com) with Deploy Hook
- Environment-specific workflows: testing for `develop`, deployment for `main`

## 🧪 Testing Workflow (CI)

- When a **Pull Request is opened against `develop`**:
  - GitHub Actions triggers the `cypress-tests.yml` workflow
  - Cypress component tests are run
  - Test results are displayed directly in the PR on GitHub

## 📦 Deployment Workflow (CD)

- When code is **merged from `develop` into `main`**:
  - GitHub Actions triggers the `deploy-to-render.yml` workflow
  - App is deployed to [Render](https://render.com) using a Deploy Hook URL

## 🛠️ Setup Instructions

### 1. Clone and Install

```bash
git clone https://github.com/cdgrosso/Github-Actions.git
npm install