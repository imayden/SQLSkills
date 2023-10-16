# SQL Practice Questions

## 1. Students Table

| SID | LastName | FirstName | Career | Program | City | Started |
|-----|----------|-----------|--------|---------|------|---------|
| 1   | Smith    | John      | Engineer | CS    | NY   | 2020    |
| 2   | Doe      | Jane      | Doctor   | Med   | LA   | 2019    |

**Question**: List all students who started after 2019.

**Expected Output**:

| SID | LastName | FirstName |
|-----|----------|-----------|
| 1   | Smith    | John      |

**Answer**: 
```
SELECT SID, LastName, FirstName 
FROM Students
WHERE Started > 2019;
```

## 2. Courses Table

| CID | CourseName | Department | CourseNo |
|-----|------------|------------|----------|
| 1   | Math       | Science    | 101      |
| 2   | Biology    | Science    | 102      |

**Question**: List all courses under the 'Science' department.

**Expected Output**:

| CID | CourseName |
|-----|------------|
| 1   | Math       |
| 2   | Biology    |

**Answer**: 
```
SELECT CID, CourseName
FROM Courses
WHERE Department = 'Science';
```

## 3. Enrolled Table

| StudentID | CourseID | Quarter | Year |
|-----------|----------|---------|------|
| 1         | 1        | Fall    | 2020 |
| 2         | 2        | Spring  | 2019 |

**Question**: List all students enrolled in courses in the year 2020.

**Expected Output**:

| StudentID |
|-----------|
| 1         |

**Answer**: 
```
SELECT StudentID 
FROM Enrolled
WHERE Year = 2020;
```

## 4. Student Groups Table

| GID | Name      | PresidentID | Founded |
|-----|-----------|-------------|---------|
| 1   | GroupA    | 1           | 2019    |
| 2   | GroupB    | 2           | 2020    |

**Question**: List all groups founded in 2019.

**Expected Output**:

| GID | Name   |
|-----|--------|
| 1   | GroupA |

**Answer**: 
```
SELECT GID, Name
FROM StudentGroups
WHERE Founded = 2019;
```

## 5. Members Table

| StudentID | GroupID | Joined |
|-----------|---------|--------|
| 1         | 1       | 2020   |
| 2         | 2       | 2019   |

**Question**: List all members who joined groups in 2020.

**Expected Output**:

| StudentID |
|-----------|
| 1         |

**Answer**: `SELECT StudentID FROM Members WHERE Joined = 2020;`

## 6. Students Table

**Question**: List all students from the city 'NY'.

**Expected Output**:

| SID | LastName | FirstName |
|-----|----------|-----------|
| 1   | Smith    | John      |

**Answer**: `SELECT SID, LastName, FirstName FROM Students WHERE City = 'NY';`

## 7. Courses Table

**Question**: List all courses with CourseNo greater than 101.

**Expected Output**:

| CID | CourseName |
|-----|------------|
| 2   | Biology    |

**Answer**: `SELECT CID, CourseName FROM Courses WHERE CourseNo > 101;`

## 8. Enrolled Table

**Question**: List all students enrolled in the 'Fall' quarter.

**Expected Output**:

| StudentID |
|-----------|
| 1         |

**Answer**: `SELECT StudentID FROM Enrolled WHERE Quarter = 'Fall';`

## 9. Student Groups Table

**Question**: List all groups with a president having SID 1.

**Expected Output**:

| GID | Name   |
|-----|--------|
| 1   | GroupA |

**Answer**: `SELECT GID, Name FROM StudentGroups WHERE PresidentID = 1;`

## 10. Members Table

**Question**: List all members of group with GID 2.

**Expected Output**:

| StudentID |
|-----------|
| 2         |

**Answer**: `SELECT StudentID FROM Members WHERE GroupID = 2;`

## 11. Students Table

**Question**: List all students with a career as 'Engineer'.

**Expected Output**:

| SID | LastName | FirstName |
|-----|----------|-----------|
| 1   | Smith    | John      |

**Answer**: `SELECT SID, LastName, FirstName FROM Students WHERE Career = 'Engineer';`

## 12. Courses Table

**Question**: List all courses with a CourseNo less than 102.

**Expected Output**:

| CID | CourseName |
|-----|------------|
| 1   | Math       |

**Answer**: `SELECT CID, CourseName FROM Courses WHERE CourseNo < 102;`

## 13. Enrolled Table

**Question**: List all students enrolled in the year 2019.

**Expected Output**:

| StudentID |
|-----------|
| 2         |

**Answer**: `SELECT StudentID FROM Enrolled WHERE Year = 2019;`

## 14. Student Groups Table

**Question**: List all groups founded after 2019.

**Expected Output**:

| GID | Name   |
|-----|--------|
| 2   | GroupB |

**Answer**: `SELECT GID, Name FROM StudentGroups WHERE Founded > 2019;`

## 15. Members Table

**Question**: List all members who joined groups before 2020.

**Expected Output**:

| StudentID |
|-----------|
| 2         |

**Answer**: `SELECT StudentID FROM Members WHERE Joined < 2020;`

## 16. Students Table

**Question**: List all students with the first name 'Jane'.

**Expected Output**:

| SID | LastName | FirstName |
|-----|----------|-----------|
| 2   | Doe      | Jane      |

**Answer**: `SELECT SID, LastName, FirstName FROM Students WHERE FirstName = 'Jane';`

## 17. Courses Table

**Question**: List all courses under the department other than 'Science'.

**Expected Output**:

| CID | CourseName |
|-----|------------|
| ... | ...        |

**Answer**: `SELECT CID, CourseName FROM Courses WHERE Department <> 'Science';`

## 18. Enrolled Table

**Question**: List all students enrolled in the 'Spring' quarter.

**Expected Output**:

| StudentID |
|-----------|
| 2         |

**Answer**: `SELECT StudentID FROM Enrolled WHERE Quarter = 'Spring';`

## 19. Student Groups Table

**Question**: List all groups without a president having SID 2.

**Expected Output**:

| GID | Name   |
|-----|--------|
| 1   | GroupA |

**Answer**: `SELECT GID, Name FROM StudentGroups WHERE PresidentID <> 2;`

## 20. Members Table

**Question**: List all members of group with GID 1.

**Expected Output**:

| StudentID |
|-----------|
| 1         |

**Answer**: `SELECT StudentID FROM Members WHERE GroupID = 1;`

---

**Note**: The above questions are based on the provided PDF content and are designed for practice purposes. Always refer to specific database documentation for detailed information and nuances.
