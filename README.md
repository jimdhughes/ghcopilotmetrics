# Random exploration thing
## Purpose
My PowerBI broke because the API changed - I was using this one: https://github.com/github-copilot-resources/copilot-metrics-viewer-power-bi

The new APIs are here:
https://docs.github.com/en/enterprise-cloud@latest/rest/copilot/copilot-usage-metrics?apiVersion=2022-11-28

## Environment variables
create a .env or set the following environment variables
```bash
BEARER_TOKEN=""
ENTERPRISE_NAME=""
```
Note: bearer token needs to have appropriate permissions defined in the docs

## Usage
Run the cells, it creates a graph I'm interested in and outputs some usage details. Data saves to a `.data/` folder. Use that for powerbi and stuff.

## Better things to do
- Ingest this into your datalake on regular intervals. Maybe use the 1-day option to run a pipeline daily instead of running 28 days every time. Really, the world is your oyster