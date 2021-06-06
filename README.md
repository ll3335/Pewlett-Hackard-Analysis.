# Pewlett-Hackard-Analysis.

## Overview of The Analysis
This analysis aims at determining the number of retiring employees per title and identify employees who are eligible to participate in a mentorship program.



## Results
- Retirement Titles
<img width="755" alt="Screen Shot 2021-06-06 at 4 41 22 PM" src="https://user-images.githubusercontent.com/82549066/120939555-90db4900-c6e6-11eb-9338-343ecdcce021.png">

The image above illustrates retiring employee's information about employee number, name, title and working date.

- Retirement Titles (Unique)
<img width="569" alt="Screen Shot 2021-06-06 at 4 41 41 PM" src="https://user-images.githubusercontent.com/82549066/120939690-2c6cb980-c6e7-11eb-950e-5b56e11ea457.png">

The image above illustrates retiring employee's information about employee number, name, titile and working date with only one title.

- Number of Retiring Employee
<img width="247" alt="Screen Shot 2021-06-06 at 4 41 55 PM" src="https://user-images.githubusercontent.com/82549066/120939756-81a8cb00-c6e7-11eb-8c05-641373ebf3f8.png">

The image above illustrates the number of retiring employee grouped by titles.

- Mentorship Eligibility
<img width="836" alt="Screen Shot 2021-06-06 at 4 42 35 PM" src="https://user-images.githubusercontent.com/82549066/120939782-ac931f00-c6e7-11eb-8213-d80520915f58.png">

The image above illustrates employees who are eligible for the mentorship program.



## Summary
- Silver Tsunami Impact
```
SELECT COUNT(uni.title)
FROM unique_titles as uni
```
<img width="105" alt="Screen Shot 2021-06-06 at 5 05 59 PM" src="https://user-images.githubusercontent.com/82549066/120940103-7ce51680-c6e9-11eb-8b7c-1d8f1845f5b5.png">

There are around 90, 389 employees need filled as the 'silver tsunami' begins to make an impact. (Code and image for counting of roles are provided above.)

- Next Generation Mentor Problem
```
SELECT COUNT(men.emp_no)
FROM mentorship_eligibility as men
```
<img width="102" alt="Screen Shot 2021-06-06 at 5 08 36 PM" src="https://user-images.githubusercontent.com/82549066/120940156-e1a07100-c6e9-11eb-93bd-a2e268d608dc.png">

There will be not enough mentors for the nest generation employees as there are only 1, 549 mentors and 90, 389 roles need filled. Each mentor need carry for 58 employee which is not realistic. (Code and image for counting of eligible mentors are provided above.)
