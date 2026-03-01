# Action Repository

This repository triggers GitHub webhook events that are processed by the webhook-repo Flask application.

## Purpose
- Source repository for GitHub webhook testing
- Triggers webhook events on push, pull request, and merge actions
- Used for the GitHub Webhook Processor assessment project

## Setup
1. This repository is already configured to send webhooks to webhook-repo
2. Make changes and push to trigger webhook events
3. Check webhook-repo dashboard to see processed events

## Webhook Configuration
- **Payload URL**: Configured in webhook-repo
- **Content Type**: `application/json`
- **Events**: Pushes, Pull requests, Pull request merges
- **Secret**: Matches webhook-repo configuration

## Usage
```bash
# Make changes and push to trigger webhooks
git add .
git commit -m "Test webhook trigger"
git push origin main

# Create a pull request
git checkout -b feature-branch
# Make changes...
git push origin feature-branch
# Create PR on GitHub
```

## Event Types Generated
- **Push Events**: When code is pushed to any branch
- **Pull Request Events**: When PRs are opened, updated, or merged
- **Merge Events**: When branches are merged

## Monitoring
Check the webhook-repo dashboard to see real-time event processing.
