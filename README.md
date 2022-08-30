# Azure DevOps - Self-hosted agent

## Quickstart

Build:

```bash
docker build -t devops-agent:latest .
```

Run:

```bash
docker run -e AZP_URL='https://dev.azure.com/<DevOps Org>' -e AZP_TOKEN='<PAT token>' -e AZP_AGENT_NAME=dockerdevopsagent -e AZP_POOL='Default' devops-agent:latest 
```

[Reference](https://docs.microsoft.com/en-us/azure/devops/pipelines/agents/docker?view=azure-devops#linux)
