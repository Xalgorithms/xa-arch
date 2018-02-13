# Summary

As documented in detail elsewhere, the projects managed by the
Foundation fall into three high-level categories:

- Lichen: A UBL document processing system that sends business
  documents to the XADF for rule discovery and execution. This
  categories includes web and mobile applications that interact with
  Lichen document services.
  
- XADF: The XA Data Fabric - A compute service that performs rule
  discovery and execution for hierarchical documents (JSON).
  
- Authoring: A Jupyter-based authoring interface for tables and rules
  used by the XADF.
  
# Active Projects

| Name                   | Category      | Language   | Core Technologies | Description                                                                                                    |
|------------------------|---------------|------------|-------------------|----------------------------------------------------------------------------------------------------------------|
| xa-arch                | Documentation | Markdown   |                   | Shared documentation used in each category                                                                     |
| xa-assembly            | Common        | YAML       | Docker            | Tools and and Dockerfiles for common shared containers                                                         |
| xa-rules               | Common        | Ruby       | Parslet           | Common library for parsing XAlgo rules.                                                                        |
| xa-ubl                 | Common        | Ruby       |                   | Common library for parsing UBL documents.                                                                      |
| xadf-compute-functions | XADF          | Scala      | Spark, Kafka      | The core functionality of the Data Fabric. Includes jobs that implement the [pipeline process](./pipeline.md). |
| xadf-deploy            | XADF          | Ruby, YAML | Docker            | Deployment and testing scripts / tools for the XADF                                                            |
| xadf-revisions-service | XADF          | Ruby       | Sinatra           | Monitors GitHub (or other SCM systems) for new rules added by the Authoring UI                                 |
| xadf-schedule-service  | XADF          | Ruby       | Sinatra           | Part of the public API for the XADF. External requests for process are asynchronously submitted here.          |
| xadf-examples-general  | XADF          | XAlgo      |                   | Common examples demonstrating the Fabric                                                                       |
| xadf-query-service     | XADF          | Ruby       | Sinatra           | Service offering public API for retrieving data synchronously from the Fabric.                                 |
| xadf-respond-service   | XADF          | Javascript | NodeJS            | A WebSocket service that outputs notifications related to submitted requests                                   |
| documents-service      | Lichen        | Ruby       | Grape             | A webservice used by the Lichen applications to process UBL and submit it to the Fabric                        |
| lichen-deploy          | Lichen        |            |                   | Deployment tooling for Lichen applications                                                                     |




