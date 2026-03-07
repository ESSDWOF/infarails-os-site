# Infarails OS Site

This repository contains the source code for the Infarails OS website.

## Deployment

This project uses GitHub Actions for automated deployment to the IONOS VPS. Every push to the `main` branch will trigger a deployment.

### Required GitHub Secrets

Before deployments can work, you need to add the following secrets to your GitHub repository:

1. **VPS_HOST** - The hostname or IP address of your IONOS VPS
2. **VPS_USER** - The SSH username for connecting to the VPS
3. **VPS_SSH_KEY** - The private SSH key for authentication (without passphrase recommended)

To add secrets:
1. Go to the repository settings on GitHub
2. Navigate to Secrets and variables > Actions
3. Click "New repository secret" and add each secret

### Deploy Path

The website is deployed to: `/var/www/infarails`

