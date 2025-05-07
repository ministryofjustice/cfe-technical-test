# Centre for Excellence - Lead Data Engineer Test

### Task Introduction
You are the lead Data Engineer working on a pilot programme to improve the analytical data available to police forces. Your task is to create a dataset to enable analysts to explore the relationship between police 'stop and search' events and the number of police officers on patrol.

Derbyshire police force have supplied some sample patrol data and you need to combine this with their public stop and search data.

We expect this pilot to expand to include more police forces and various time frames. You are also expected to lead the team in establishing and maintaining coding and deployment standards and this should be reflected in your code as well as any additional processes you create.

You have 5 tasks to complete over the next 60 minutes. You are free to write and structure your code as you see fit. You will be required to present your solution, describe what you have done, how you have done it and why you made each choice.

### 1. Create a process for establishing and maintaining code quality
It is important that this project aligns to PEP 8 standards and other industry best practices. Please implement the core of a framework to ensure all code committed to this project aligns to a set of standards you have selected.


### 2. Ingest the public 'stop and search' data
This can be found here: https://data.police.uk/docs/ under 'Stop and searches by force'.
We require the data for April 2024, May 2024 and June 2024 for the 'Derbyshire' police force.
The code for the Derbyshire police force is 'derbyshire'.

If you are unable to load this data for any reason, you can find a copy in `raw_data` as `04_stop_and_search.json`, `05_stop_and_search.json` and `06_stop_and_search.json`. Please retain any code you have written.


### 3. Load the patrol data
This is a static excel file stored in the repo at this location: `raw_data/derbyshire_patrol_data.xlsx`.


### 4. Clean and filter the data.
The 'stop and search' data should be filtered to only include records which:
- have a populated 'age_range' value

The patrol data must:
- Exclude any days with missing data


### 5. Create a framework for ensuring that code stored in git maintains the required standards
It is important for code that is deployed to production and is worked on by multiple team members to adhere to agreed standards. Please implement a framework to ensure that code merged into main, via pull requests, is correct and meets these standards.
