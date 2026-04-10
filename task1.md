# SQL Joins Practice: Data Integration

**Objective:** To merge data from 'Students' and 'Projects' tables using various SQL Join techniques.

### 1. Sample Tables
- **Students Table:** `student_id`, `name`, `course`
- **Projects Table:** `project_id`, `student_id`, `project_title`

### 2. SQL Join Queries & Logic

#### A. INNER JOIN
*Fetches only the records that have matching values in both tables.*
```sql
SELECT Students.name, Projects.project_title
FROM Students
INNER JOIN Projects ON Students.student_id = Projects.student_id;
