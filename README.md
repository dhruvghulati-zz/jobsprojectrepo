# Jobs Salary Cleaning Script

A personal data project to clean and summarise salaries from jobs data obtained via import.io.

##Background

There have been many attempts to use salary data to help inform what different job types should earn in a marketplace.
This type of information is key if companies operate an open salary policy, that is that each employee should be paid
the market rate of what they are worth, nothing less.

There have been other [data science projects](http://nycdatascience.com/students-work/job-salary-prediction-with-python/)
to help predict job salary based on other schema e.g. job description, title,
industry etc. There is also a famous Kaggle competition on this.

* https://www.kaggle.com/c/job-salary-prediction

##Output

My iPython notebook (work in progress) is available [here] (http://nbviewer.ipython.org/github/dhruvghulati/jobsprojectrepo/blob/master/jobsproject.ipynb)
. This project uses a month of python knowledge from Team Treehouse's online course. 

I wanted to use this project to learn new libraries and tools e.g. PyCharm, pandas, numpy, SciPy, and ipython. The project
also involved some Regular Expressions knowledge. I wanted to apply my learnt tools for a practical need, and hack around.

##PseudoCode

The structure of the code written so far is:

1. Build APIs to job boards using import.io batch search
2. Run them using Google sheets to generate CSVs to each job boards with multiple schema
3. Use iPython notebook as the baseline for my code
4. Combine CSVs into one dataframe in pandas
5. Find the salary column and split by delimiter
6. Find the min and max salaries, and assign them to new split dataframes
7. Merge the salary dataframe into the main dataframe.

##Room for improvement

There are many ways I want to improve this project:

* Build a cleaning script to clean a CSV that has been appended from multiple CSVs with differently ordered columns, headers maintained.
* Run APIs in a consistent manner using dual APIs in a pagination script (not have to use Google sheets to produce CSVs)
* Learn Beautiful Soup or Scrapy
* Move my work towards predictive analytics/machine learning
* Account for the context of a job from job description - one product manager role may be more senior than another, one startup
role may be sexier than another.
* Deduplication of jobs obtained
* Provide value to benefits and medical insurance in a quantitative manner
* Account for and remove generic job adverts e.g.“Searching for Oracle Consultants“, which do not refer to one job role
* Use mysql for the cleaned data to then create sub-tables and pivottables for my data.
