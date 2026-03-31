#  Student Data Analysis in R

##  Overview

This project presents a comprehensive data analysis of a student dataset using **R**. The goal of the analysis is to explore relationships between study habits and academic performance, as well as to apply statistical methods and data visualization techniques.

The project was created as part of a university coursework assignment focused on practical data analysis.

---

##  Dataset

The dataset contains information about **500 students** and includes the following variables:

* **Student ID** – unique identifier
* **Gender** – Female / Male
* **Field of Study** – Computer Science, Economics, Psychology, Biology
* **Age** – student age
* **Study Time** – number of study hours per week
* **Grade Average** – student's GPA

---

##  Features & Analysis

###  Data Preparation

* Imported data from Excel using `openxlsx`
* Converted categorical variables into factors
* Identified qualitative and quantitative variables
* Handled missing values:

  * Numerical → replaced with mean
  * Categorical → replaced with most frequent value

---

###  Exploratory Data Analysis (EDA)

* Summary statistics for all variables
* Distribution analysis (histograms, density plots)
* Skewness and symmetry evaluation
* Visualizations using **ggplot2**:

  * Histograms
  * Boxplots
  * Bar charts

 **Key findings:**

* Study time varies depending on the field of study
* Biology students study the most on average
* Economics students study the least
* Computer Science shows the highest variability

---

###  Statistical Modeling

* Correlation analysis between study time and GPA

* Linear regression model:

  ```
  Study Time ~ Grade Average
  ```

* Model diagnostics:

  * Residual analysis
  * Shapiro-Wilk test (normality)
  * Breusch-Pagan test (homoscedasticity)
  * Durbin-Watson test (autocorrelation)

 

---

###  Distribution Analysis

* Fitting theoretical distributions to study time data
* Comparison of multiple distributions (normal, gamma, log-normal, etc.)
* Parameter estimation and goodness-of-fit evaluation

---

###  Scholarship Function

A custom R function was implemented to calculate scholarships based on GPA:

| GPA Threshold | Scholarship |
| ------------- | ----------- |
| ≥ 4.5         | 750 PLN     |
| ≥ 4.7         | 850 PLN     |
| ≥ 4.9         | 950 PLN     |

The function returns:

* Number of awarded scholarships
* List of students with scholarship amounts
* Total monthly cost

---

##  Technologies Used

* **R**
* **R Markdown**
* Libraries:

  * `ggplot2`
  * `openxlsx`
  * `Hmisc`
  * `fitdistrplus`
  * `car`

---

##  How to Run

1. Clone the repository
2. Open the `.Rmd` or `.R` file in RStudio
3. Install required packages:

   ```r
   install.packages(c("ggplot2", "openxlsx", "Hmisc", "fitdistrplus", "car"))
   ```
4. Run the script or knit the R Markdown file

---

##  Project Goals

* Practice data cleaning and preprocessing
* Perform exploratory data analysis
* Apply statistical modeling techniques
* Validate model assumptions
* Create meaningful visualizations
* Develop reusable analytical functions

---

##  Author

**Alicja Czuż**

---

##  License

This project is created for educational purposes.
