# Pewlett-Hackard-Analysis
## Overview
This analysis focuses on employees that are likely to retire in the next few years and how many positions Pewlett Hackard needs to be prepared to fill. This analysis helps future proof Pewlett Hackard by generating lists of all employees eligible for a retirement package. 


## Results
- Senior Engineers and Staff make up 64% of roles eligible for retirement packages 

- Of 90,398 roles eligible for retirement packages only 2 are Managers

- Assistant Engineers are less likely to be of retirement age than other engineering roles

- There are no birth dates listed in 1965 after 2/1/1965. There may be an inconsistency in the data for eligible mentors. 

## Summary
Based on a count of the unique_titles table (code below), 90,398 roles are currently held by employees eligible for a retirement package. 

- SELECT COUNT(emp_no)  
  from unique_titles;

By running the below query we can see that there according to current records there are 1549 employees eligible to be mentors. Contrasted to the 90,398 roles currently eligible for retirment the ratio of current mentors to roles available would be 58 to 1. Pewlett Hackard likely needs to expand mentor eligibility requirements outside of those only born in 1965.

- SELECT COUNT(emp_no)  
  from mentorship_eligibility;
