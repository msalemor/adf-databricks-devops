# ADF and Databricks DevOps

A DevOPs guide for ADF and Databricks

## ADO Configuration

- Connect ADF to ADO
- Connect Databricks to same ADO

### Creating or modifying an ADF pipeline with a Databricks notebook

- One of the developers creates a feature branch from ADF or Databricks
- Have the Data Bricks checout the brand and work on the notebook and data
- Have the ADF developer checkout the same feature branch from the repo and work on the ADF pipeline
- Collaborate to create the pipeline with the Databricks notebook
- Once tested, one of the developers should submit the pull request
- Upon approval both the ADF json and Databricks code is merged into main
- In ADF, publish the pipeline

## CD to Upper Environment(s)

### ADF

- Generates ARM templates
- Use a pipeline to push the ARM templates to upper environment(s)
  - Modify the parameters as appropritly

### Databricks

- Generates code and data files
- Use a pipeline (using the Databricks tools) to push the code required files to the upper environment(s)
  - Modify parameter and data as appropritly
