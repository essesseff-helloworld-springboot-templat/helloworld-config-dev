# hello-world Config - DEV

Helm chart for DEV environment.

## Configuration

- **Environment**: DEV
- **Auto-Deploy**: Yes (via essesseff upon successful code build triggered by source code push)
- **Namespace**: `essesseff-hello-world-flask-template`
- **Ingress**: `example.com/hello-world-dev`

## Updates

This repository in combination with the argocd-env environment-specific deployment config determine when/if/how deployments occur via Argo CD. This repository is updated by essesseff platform when DEV deployments are to occur as per Developer manual decision and/or subsequent to successful code build typically triggered by source code push.

Typically, only the values.yaml file should be manually altered, while any/all other changes in the repository are made via essesseff deployment orchestration.
