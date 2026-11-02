
Page
1
of 2
# StudyQuest
## Team Information
### Team Members
- Keerthi 
- Arwa 
- Esther
- Vishwa
- Sarah
---
## Project Description
### Domain: Productivity
StudyQuest is a student productivity website with a cozy game where students organize their courses, assignments, deadlines, and daily tasks, and use a built-in study timer to track focus on work. Productivity becomes gamified with completing tasks and study sessions earns XP and coins, which the student uses to level up their character, keep streaks, and customize a virtual room with a pet.

# Problem 
Students often struggle with motivation, procrastination, and consistent study habits and traditional productivity apps help organize responsibilities but don't make completing them rewarding. However, StudyQuest adds rewards to complete academic work which makes it fulfilling. 
---
## User Stories
### As a student taking several courses, I want to organize my assignments by course so that I can see what work belongs to each class.
### As a student with many upcoming deadlines, I want to record when each assignment is due and how important it is so that I know what to work on first.
### As a student who struggles with motivation, I want to be rewarded when I finish a task so that completing my work feels satisfying.

---
## Use Cases
### Use Case 1: Add Course
**Primary Actor:** Student
**Precondition:** The student is logged in.
**Trigger:** The student chooses to add a course.
**Main Success Scenario:**
1. Student provides a course code and course name.
2. System checks that the course code is not already in use.
3. System saves the course.
4. System presents the updated course list.

**Extensions:**
- 1a. Student cancels → no course is added → use case ends.
- 2a. Course code or name is empty → system reports the missing information → return to step 1.
- 2b. Course code already exists → system reports the duplicate → return to step 1.

**Success Outcome:** The new course appears in the student's course list.

### Use Case 2: Add Task
**Primary Actor:** Student
**Precondition:** The student has at least one course (or uses the default "General" list).
**Trigger:** The student chooses to add a task.
**Main Success Scenario:**
1. Student chooses the course the task belongs to.
2. Student provides a title, due date, and priority level.
3. System validates the information.
4. System saves the task under the chosen course.
5. System presents the task in the upcoming tasks list, ordered by due date and priority.

**Extensions:**
- 2a. Student cancels → no task is added → use case ends.
- 3a. Title is empty → system reports the missing title → return to step 2.
- 3b. Due date is in the past → system asks the student to confirm → if confirmed, continue at step 4; otherwise return to step 2.

**Success Outcome:** The task is stored under the chosen course and shown in the upcoming tasks list.


### Use Case 3: Complete Task
**Primary Actor:** Student
**Precondition:** The task exists and is not yet complete.
**Trigger:** The student chooses to mark a task as complete.
**Main Success Scenario:**
1. Student chooses the task to complete.
2. System marks the task as complete.
3. System calculates the XP and coins earned based on the task's priority, whether it was on time, and the current streak.
4. System adds the rewards to the student's character and updates the streak.
5. System presents the rewards earned and the updated level progress.

**Extensions:**
- 3a. Task is overdue → system calculates a reduced reward → continue at step 4.
- 4a. Character's XP reaches the next level threshold → system levels up the character and presents a level-up message → continue at step 5.

**Success Outcome:** The task is marked complete, and the character's XP, coins, and streak reflect the reward.


### Use Case 4: View Progress Dashboard
**Primary Actor:** Student
**Precondition:** The student is logged in.
**Trigger:** The student chooses to view their progress.
**Main Success Scenario:**
1. Student opens the progress dashboard.
2. System retrieves the student's level, XP, coins, streak, tasks completed, and total study time.
3. System presents these statistics, including study time per course.

**Extensions:**
- 2a. Student has no recorded activity → system presents a message encouraging them to complete their first task → use case ends.

**Success Outcome:** The student sees their current progress statistics.


### Use Case 5: Run Study Session
**Primary Actor:** Student
**Precondition:** The student has at least one course.
**Trigger:** The student chooses to start a study session.
**Main Success Scenario:**
1. Student chooses a course and a session length.
2. System starts the timer and presents the remaining time.
3. Timer reaches zero.
4. System records the session and calculates XP based on its length.
5. System adds the XP to the character and updates the streak and total study time.
6. System presents the XP earned.

**Extensions:**
- 2a. Student pauses the session → timer stops until the student resumes → continue at step 2.
- 2b. Student ends the session early → system records only the minutes completed → continue at step 4.
- 4a. Session lasted under 5 minutes → system records the session but awards no XP → use case ends.

**Success Outcome:** The study session is recorded, and the character's XP, streak, and total study time are updated.

(Add additional use cases as needed.)
---
## Minimal Viable Product (MVP)
| Team Member | MVP Use Case |
|-------------|--------------|
| Keerthi  | Use Case |
| Name | Use Case |
| Name | Use Case |
| Name | Use Case |
| Name | Use Case |
---
## Entities
### Entity 1
### Entity 2
(Add additional entities as needed.)
---
## API Usage
**API Name:**
**Documentation:** [Link]
**How it is used in the program:**
---
## Design Diagrams
### UML Class Diagram
### Sequence Diagrams
---
## How to Run
TO DO [Instructions for running the program.]
---
## Notes
[Any additional]
