# Centre for Excellence - Lead Data Engineer Test

### Task Introduction
You are the lead Data Engineer working on a pilot programme to improve the analytical data available to police forces. Your task is to implement the initial data ingestion and establish a code repository that will maintain a high standard of code and working practices. A basic project framework has been provided.

You do not need to push your code to GitHub, or deploy it any where.

We expect this pilot to expand to include more police forces and cover additional time frames and your approach to writing code should anticipate this.
The project team will include colleagues with a range of knowledge and experience. You should focus on creating frameworks, workflows, documentation and processes to support the growth of this team and maintenance of standards.

The data comprises public 'stop and search' data from an API and dummy police patrol data supplied by Derbyshire police force.

You have 4 tasks to complete over the next 45 minutes. You are free to write and structure your code as you see fit.
After the 45 minutes, you will have 5 minutes to present your work during which you will describe what you have done and why.
There will then be an additional coding task to complete live with the interview panel.

### 1. Introduce a mechanism for managing project dependencies
This pipeline will be deployed into a cloud environment and be worked on by many team members. Please introduce a mechanism to ensure that the correct dependencies are used and maintained for this project.

You can assume that the minimum critical dependencies are pandas/polars and pytest.

### 2. Ingest the public 'stop and search' data
This can be found here: https://data.police.uk/docs/ under 'Stop and searches by force'.
We require the data for April 2024, May 2024 and June 2024 for the 'Derbyshire' police force.
The code for the Derbyshire police force is 'derbyshire'.

Please convert this data to a DataFrame so that it can be combind with the patrol data.

If you are unable to load this data for any reason, you can find a copy in `raw_data` as `04_stop_and_search.json`, `05_stop_and_search.json` and `06_stop_and_search.json`. Please retain any code you have written.

### 3. Load the patrol data
This is a static csv file stored in the repo at this location: `raw_data/derbyshire_patrol_data.csv`.
Please ensure that only the required rows of data are included in the DataFrame.

### 4. Create a process for establishing and maintaining code quality
Code deployed to production, and worked on by multiple people, must adhere to agreed standards.
This project must align with PEP8 standards and other industry best practices for productionised python code.

Please implement any processes/workflows to ensure that all code committed to this project align to a set of standards you have selected. 
This should include all code sent to the remote repository, including pull requests.
