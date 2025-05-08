
[COE891 - Final Project Report - Group 2 (1).pdf](https://github.com/user-attachments/files/20107485/COE891.-.Final.Project.Report.-.Group.2.1.pdf)
TEAMMATES Testing Project - Syed Abdul Wadood's Contribution
Overview
This project involved comprehensive testing of TEAMMATES, a cloud-based peer evaluation tool, using various software testing methodologies. My contributions focused on implementing graph-based testing, mutation testing, and input space partitioning (ISP) testing for critical Java classes in the system.

Key Contributions
1. Graph-Based Testing (CFG and DFG)
Designed Control Flow Graphs (CFG) and Data Flow Graphs (DFG) for multiple methods

Achieved 100% statement, branch, and path coverage for:

publishFeedbackSession()

getSectionsNameForCourse()

validateSectionsAndTeams()

isStudentInTeam()

Developed comprehensive test cases mapping to all CFG paths

2. Mutation Testing
Implemented mutation testing using PIT (Pitest) framework

Achieved high mutation coverage (87/109 mutants killed) across:

StudentsLogic class (91% line coverage)

CoursesLogic class (89% line coverage)

FeedbackSessionLogic class (100% line coverage)

Created test cases to kill mutants and improve test strength

3. Input Space Partitioning (ISP) Testing
Designed test cases based on input characteristics for:

getTeamsForSection()

getSectionsNameForCourse()

getTeamsForCourse()

getCoursesForInstructor()

Created decision tables to ensure complete input space coverage

Achieved 90%+ coverage for all ISP-tested methods

Technical Skills Demonstrated
Testing Methodologies: CFG/DFG analysis, mutation testing, ISP testing

Tools: JUnit, Mockito, PIT (Pitest), JaCoCo (for coverage)

Programming: Java

Analysis: Control flow analysis, data flow analysis, test case design

Challenges Overcome
Complex CFG/DFG Construction: Manually creating accurate graphs for methods with nested conditions and exception handling

Mutation Testing Integration: Configured PIT for Java compatibility and analyzed mutant survival

Test Isolation: Implemented mock objects to isolate unit tests from dependencies

Complete Coverage: Ensured all logical paths were tested through systematic analysis

Key Achievements
Contributed to overall project success with 80%+ line coverage

Identified critical bugs through mutation testing

Developed maintainable test suites with clear documentation

Created visual representations of control and data flows for complex methods

Files Contributed
StudentsLogicTest.java - Mutation and graph-based tests

CoursesLogicTest.java - ISP and graph-based tests

FeedbackSessionLogicTest.java - Comprehensive test suite

Test documentation and CFG/DFG diagrams

How to Run Tests
Clone the repository

Install dependencies:

bash
mvn install
Run specific test suites:

bash
mvn test -Dtest=StudentsLogicTest
Generate mutation reports:

bash
mvn org.pitest:pitest-maven:mutationCoverage
Reflections
This project provided valuable hands-on experience with advanced testing techniques in a real-world application. The systematic approach to test design improved the reliability of the TEAMMATES system while deepening my understanding of software quality assurance best practices.
