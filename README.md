# Morel Workflows
A collection of workflows developed for Morel Technology.

## Deploy Dart Frog API
Builds and deploys a Dart Frog API to Google Cloud Run.

### Inputs
- project_id:
  - description: "The GCP id the action should deploy to."
  - required: true
  - type: string
- service:
  - description: "The name of the service being deployed."
  - required: true
  - type: string
- region:
  - description: "The region to deploy this service to."
  - required: true
  - type: string
- environment_variables:
  - description: "The environment variables for this service."
  - required: false
  - type: string
- flags:
  - description: "Additional flags to add to gcloud run deploy."
  - required: false
  - type: string
- code_path:
  - description: "Path where the Dart Frog API is located."
  - required: false
  - type: string
  
## Secrets
- GCP_SA_KEY:
  - required: true
## Outputs
- url:
  - description: "The URL of the deployed service"
