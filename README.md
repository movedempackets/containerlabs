#### Containerlabs

A repo containing containerlab clab files. Using on demand pipelines to validate, deploy and delete labs. Born out of the frustration of repetitive lab building and a lack of tooling to manage labs in a devops fashion.

--

The repository includes two workflows: 

1. `ci.yml` runs automated json schema validation on lab definition files (`*.clab.yml`). This workflow uses github hosted runners.
2. `cd.yml` uses workflow dispatch with both command and lab directory inputs to deploy or destroy labs. This workflow uses self hosted runners. 
