# ADF and Data Bricks DevOps

A DevOPs guide for ADF and Data Bricks

## ADO Configuration

- Connect ADF to ADO
- Connect Data Bricks to same ADO

### Creating a new ADF pipeline with Data Bricks

- Create a feature branch
- Have the Data Bricks developer work on notebook and data
- Have the ADF developer checkout the same feature branch from the repo and work on the pipeline
- Collaborate to create the pipeline with the Data Bricks dependency.
- Once tested, one of the developers should submit the pull request
- Upon approval both the ADF json and Data Bricks code would be merged into main
- In ADF, publish the pipeline

## CD to Upper Environment(s)

### ADF

- Generates ARM templates
- Use a pipeline to push the ARM templates to upper environment(s)
- Modify the parameters as appropritly

### Data Bricks

- Generates code and data files
- Use a pipeline to push the code required files to the upper environment(s)
- Modify parameter and data as appropritly
