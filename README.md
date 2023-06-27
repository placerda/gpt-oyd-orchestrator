# gpt on your data orchestrator

## Quick start - Deploy to Azure

**1) Pre-reqs**

- Azure Funcion App
- Cognitive Search Service
- Index created by [ingestion](https://github.com/placerda/gpt-oyd-ingestion)
- CosmosDB Service
- Python and PIP 3

**2) Set Application Settings**

- Rename [local.settings.json.template](local.settings.json.template) to ```local.settings.json``` and update environment variables in this file to run orchestrator locally.
 
- In Azure Portal > Function App > Configuration > Application Settings: add the same variables you updated in locall.settings.json.

**3) Deploy to Azure** (this step can be repeated whenever you make changes to the front)

In VSCode with [Azure Function App Extension](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-azurefunctions) go to the *Azure* Window, reveal your Function App in the resource explorer, right-click it then select *Deploy*.