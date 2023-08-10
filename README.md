# Data Exploration Project - Employee Attrition Analysis

This project focuses on exploring employee attrition data from the "employee_attrition.csv" dataset. The code utilizes the `pandas`, `matplotlib`, and `seaborn` libraries for data analysis and visualization.

# Employee-Attrition
<hr>

Data dictionary: 

**EmployeeID**:Unique ID for each employee <br>
**recorddate_key**: The year that this record has been documented <br>
**birthdate_key**: Employee birthday <br>
**orighiredate_key**: The hire date <br>
**terminationdate_key**: The termination date <br>
**age**: Employee Age <br>
**length_of_service**: Employee length of service <br>
**city_name**: City <br>
**department_name**: Department <br>
**job_title**: Job title <br>
**store_name**: Store number  <br>
**gender_short**: Gender code <br>
**gender_full**:Gender <br>
**termreason_desc**: Termination reason <br>
**termtype_desc**: Termination type <br>
**STATUS_YEAR**: Record year <br>
**STATUS**: Terminated or active <br>
**BUSINESS_UNIT**: business unit <br>
## Getting Started

1. Make sure you have Python installed along with the required libraries (`pandas`, `matplotlib`, `seaborn`).
2. Clone this repository to your local machine.
3. Download the "employee_attrition.csv" dataset and place it in the repository directory.

## Code Overview

The code in this project covers the following steps:

### Data Loading and Initial Exploration

- The data is loaded using `pandas.read_csv()` and date columns are parsed.
- Initial data exploration is performed using `data.shape`, `data.head()`, and `data.tail()` to understand its structure and content.
- Information about the dataset, data types, and memory usage is obtained using `data.info()`.

### Data Preprocessing

- Duplicate rows are removed using `data.drop_duplicates()` to ensure data integrity.
- The `gender_full` column is dropped since it's redundant with `gender_short`.

### Feature Engineering

- The job titles are categorized into hierarchical levels, such as "Employee," "Manager," "Executive," and "Board," using predefined categories.
- A new feature, `Hierarchy`, is added to the dataset to represent these hierarchical categories.

### Data Visualization

- Data visualizations are created using `matplotlib` and `seaborn` to gain insights into employee attrition.
- Scatter plots are used to compare age and length of service for active and terminated employees.
- `FacetGrid` is used to visualize age and length of service by hierarchy, gender, and termination reasons.
- Bar plots show the distribution of terminations over different years and termination reasons.
- Count plots reveal the distribution of terminations by gender, termination type, business unit, and hierarchy.
- Histograms display the distribution of terminations across different store names.

## Conclusion

This data exploration project provides insights into employee attrition trends based on various attributes such as age, length of service, hierarchy, gender, termination reasons, business unit, and more. The visualizations and analyses can help identify patterns and factors contributing to employee attrition.

## Acknowledgments

The dataset used in this project is provided by zep-analytics and can be found in the file "employee_attrition.csv."

## License

This project is licensed under the [MIT License](LICENSE).







