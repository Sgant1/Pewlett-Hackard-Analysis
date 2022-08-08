# Overview of the Analysis

Now that Bobby has proven his SQL chops, his manager has given both of you two more assignments: determine the number of retiring employees per title, and identify employees who are eligible to participate in a mentorship program. Then, you’ll write a report that summarizes your analysis and helps prepare Bobby’s manager for the “silver tsunami” as many current employees reach retirement age.

The initial goal of this project was to determine how many employees are near retirement age to avoid a multitude of resignations without backfills prior to these individuals retiring. To do this we gathered 6 different csv files that were provided as data and merged, created, consolidated and imported data into other csv files to present consumable information to management so they can look to backfill needed positions prior to current employees retirement.

# Results

- Retiring Employees by Title was put together by showing all employees born between 1/1/1952 and 12/31/1955 along with their current titles. The reason for this was to target the "more likely" candidates for retirement. Code: ![image](https://user-images.githubusercontent.com/107363048/183336439-a51021fe-2dbf-43cf-ac17-2b8a179bd282.png)

This code gave us retirement_titles.csv - This game first name, last name, title, emp_no, and birth date.

- Additionally we further refined potential retirement candidates by using the following code: ![image](https://user-images.githubusercontent.com/107363048/183336669-63e73d88-f5f0-41b6-8f90-ad48f136819a.png)

This allowed us to remove duplicates if someone had multiple titles in their tenure or was promoted. By using to date 1/1/9999 it gives us their most up to date title.

- Lastly, we were asked to summarize this data for viewing purposes:  

![image](https://user-images.githubusercontent.com/107363048/183337055-715b9212-3deb-4cf0-bee8-bcaddaf475a2.png)

![image](https://user-images.githubusercontent.com/107363048/183337175-a07e8da4-be86-4461-866f-86712940621c.png)

Based on these summarized data points we can determine the following:

1. The staff close to retirement is almost 72k people in the unique_titles report.
2. Of this two groups are going to take the bulk of backfills.
  - Senior Engineers
  - Senior Staff
  
  Pewlett Hackard now asked us to review what employees would be available for a mentorship program. We did this with the following code:
  
  ![image](https://user-images.githubusercontent.com/107363048/183337515-0569a8eb-de40-4cd5-a1dc-213075202815.png)

1. By running this code, we were able to determine that 1,549 employees are currently employed and were born after 1965, therefore they should be available.

![image](https://user-images.githubusercontent.com/107363048/183337994-fc657a8e-2f3f-414c-a872-2605e99b73c5.png)

2. Senior Staff and Engineers will have the greatest impact in the mentorship program.

# Summary of Report

1. How many roles will need to be filled as the "Silver tsunami" begins to make an impact?

- Close to 72,000 roles will need to be replaced.

2. Are there enough qualified, retirement-ready employees in the departments to mentor the next generation of PH employees?

- There are not enough employees currently for a one-on-one mentorship program. However, if this was split up into groups by department/titles for one individual to coach multiple people, then they may be able to get by.
