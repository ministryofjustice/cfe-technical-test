# Centre for Excellence - Lead Data Engineer Test

### Task Introduction
You are the lead Data Engineer working on a pilot programme to improve the analytical data available to police forces. Your task is to implement the initial data ingestion and establish a code repository that will maintain a high standard of code and working practices. A basic project framework has been provided.

You do not need to push your code to GitHub, or deploy it any where.

We expect this pilot to expand to include more police forces and cover additional time frames and your approach to writing code should anticipate this.
The project team will include colleagues with a range of knowledge and experience. You should focus on creating frameworks, workflows, documentation and processes to support the growth of this team and maintenance of standards.

The data comprises public 'stop and search' data from an API and dummy police patrol data supplied by Derbyshire police force.

You have 4 tasks to complete over the next 45 minutes. You are free to write and structure your code as you see fit.
After the 45 minutes, you will have 5 minutes to present your work during which you will describe what you have done and why.

### 1. Create a process for establishing and maintaining code quality
It is important that this project aligns to PEP 8 standards and other industry best practices for productionised python code. Please implement the core of a framework to ensure all code committed to this project aligns to a set of standards you have selected.
You can assume that this project only requires pandas/polars and pytest as critical dependencies

### 2. Ingest the public 'stop and search' data
This can be found here: https://data.police.uk/docs/ under 'Stop and searches by force'.
We require the data for April 2024, May 2024 and June 2024 for the 'Derbyshire' police force.
The code for the Derbyshire police force is 'derbyshire'.

Please convert this data to a DataFrame so that it can be combind with the patrol data.

If you are unable to load this data for any reason, you can find a copy in `raw_data` as `04_stop_and_search.json`, `05_stop_and_search.json` and `06_stop_and_search.json`. Please retain any code you have written.


### 3. Load the patrol data
This is a static csv file stored in the repo at this location: `raw_data/derbyshire_patrol_data.csv`.
Please ensure that only the required rows of data are included in the DataFrame.


### 4. Create a framework for ensuring that code stored in git maintains the required standards
It is important for code that is deployed to production and is worked on by multiple team members adheres to agreed standards. Please implement a framework to ensure that code merged into main, via pull requests, is correct and meets these standards.
