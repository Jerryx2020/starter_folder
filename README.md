# Marriage Licence Statistics - Toronto

This project focuses on simulating and analyzing data from the **Marriage Licence Statistics** in Toronto using the **Open Data Toronto** platform. The workflow involves simulating datasets, gathering real data, cleaning the data, conducting tests, and generating a final report using **Quarto**.

## Project Structure

The project is organized into several key directories and scripts:

### 1. **Data Folder**:
   - `data/analysis_data/`: Contains the cleaned and analyzed dataset.
     - `analysis_data.csv`: The final dataset used for analysis.
   
   - `data/raw_data/`: Contains raw data and simulated data.
     - `raw_data.csv`: Raw data gathered from Open Data Toronto.
     - `simulated.csv`: Simulated data using a Poisson distribution.

### 2. **Other Folder**:
   - `other/llm/`: Contains a `usage.txt` file for tracking LLM usage or other notes.
   - `other/sketches/`: Contains rough sketches for planning the analysis.
     - `dataset.jpeg`: An image sketch of the desired dataset structure.
     - `graph.jpeg`: A sketch of the planned graph.

### 3. **Paper Folder**:
   - `paper.qmd`: The **Quarto** document that generates the PDF report. It includes the title, author, abstract, and analysis.
   - `references.bib`: Bibliography file used for citations in the report.

### 4. **Scripts Folder**:
   - `00-simulate_data.R`: Simulates data using the Poisson distribution with λ = 10.
   - `01-download_data.R`: Gathers data from Open Data Toronto using the **opendatatoronto** package.
   - `02-data_cleaning.R`: Cleans and processes the raw data, using functions like `separate()` and `lubridate::ymd()` for date handling.
   - `03-test_data.R`: Contains tests to validate the simulated and cleaned datasets.
   - `04-model.R`: (Optional) This script models the cleaned data for further analysis.
   - `05-replications.R`: (Optional) Replication script for rerunning analyses or simulations.

### Other Files:
- `.gitignore`: Specifies files and directories to be ignored by Git.
- `starter_folder.Rproj`: RStudio project file.
- `README.md`: This file, explaining the project setup and structure.

## Statement on LLM usage

Code was derived from a class example where they were written with the help of the auto-complete tool, Codriver. The abstract and introduction were written with the help of ChatHorse and the entire chat history is available in inputs/llms/usage.txt.

## How to Run the Project

### 1. Clone the Repository:
```bash
git clone https://github.com/Jerryx2020/starter_folder



