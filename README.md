
[COE891 - Final Project Report - Group 2 (1).pdf](https://github.com/user-attachments/files/20107485/COE891.-.Final.Project.Report.-.Group.2.1.pdf)

# TEAMMATES Testing Project - Group 2

**Course:** COE891 - Software Testing and QA (Winter 2025)  
**Instructor:** Dr. Reza Samavi  
**Team Members:** 
- Poojitha Bejugama
- Sid Muntaha  
- Aaron Panesar  
- Syed Abdul Wadood (500892009)  
- Cyrille Teupe Chekam  

## Table of Contents
- [Project Overview](#project-overview)
- [Testing Methodologies](#testing-methodologies)
- [Key Contributions](#key-contributions)
  - [Graph-Based Testing](#graph-based-testing)
  - [Mutation Testing](#mutation-testing)
  - [ISP Testing](#isp-testing)
- [Technical Implementation](#technical-implementation)
- [Results](#results)
- [Challenges & Solutions](#challenges--solutions)
- [How to Run](#how-to-run)
- [Conclusion](#conclusion)

## Project Overview
![TEAMMATES Architecture](docs/images/teammates-arch.png)

Comprehensive testing of [TEAMMATES](https://teammatesv4.appspot.com/), a cloud-based peer evaluation system. Focused on three core Java classes:
1. `StudentsLogic.java`
2. `CoursesLogic.java` 
3. `FeedbackSessionLogic.java`

## Testing Methodologies
| Methodology | Tools Used | Coverage Target |
|-------------|------------|-----------------|
| Graph-Based Testing (CFG/DFG) | JUnit 4, Manual Diagrams | 100% Path Coverage |
| Mutation Testing | PITest, MuJava | 80%+ Mutation Score |
| Input Space Partitioning | JUnit 5 | 90%+ Clause Coverage |
| Logic-Based Testing | Mockito | 95%+ Predicate Coverage |

## Key Contributions

### Graph-Based Testing
**Methods Tested:**
```java
// FeedbackSessionLogic
public FeedbackSessionAttributes publishFeedbackSession(String name, String courseId) 
public List<FeedbackSessionAttributes> getFeedbackSessionsClosedWithinThePastHour()

// StudentsLogic  
public void validateSectionsAndTeams(List<StudentAttributes> students, String courseId)
public boolean isStudentInTeam(String courseId, String teamName, String email)

// CoursesLogic
public List<String> getSectionsNameForCourse(String courseId)
