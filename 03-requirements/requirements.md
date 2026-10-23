# Week 3 - Requirements Analysis & Specification

## 1. Candidate Requirements

### 1. "People are sometimes unsure whether a camera is available."
Problem/Observation: The stakeholders have highlighted an issue about the uncertainty of whether or not the camera equipment is available or not.

### 2. "Technicians need to know what equipment is due back."
Stakeholder Need/Concern: This highlights the specific point of view for technicians and the lack of information they require to do their job efficiently.

### 3. "The system shall record the expected return date for each booking."
Candidate Requirement: The keyword "shall" is associated with candidate requirement which specifies the action the system shall perform.

### 4. "The college should build a mobile app."
Solution Idea: This is more of technological implementation solution rather than looking into the problem itself.

### 5. "We assume all users will have a college login."
Assumption: This is the base condition that is factually given.

### 6. "A lecturer wants reliable availability information before promising equipment."
Stakeholder Need/Concern which evolves into a Candidate Requirement later on: It starts off as a user goal and is a concern due to how subjective "reliable" is. Eventually, a technical candidate requirement will occur later as the statement outlines a workflow that will lead there.


## 2. Requirements Surgery Overview
"The system shall record the expected return date for each booking."

FIND: The requirement wants the system to be able to record return dates for each booking.

DIAGNOSE: The requirement does not specify who would be involved with the recording and it doesn't really say what the system actually do.

ASK: "What stakeholder would be involved in the recording of return dates for the bookings?"

REPAIR: "The system shall record an expected return date when a booking coordinator creates a new booking reservation."

CHECK: Verifying the requirement:
1. WHO is involved? The booking coordinator.
2. WHAT must the system do? Automatically records the expected return date.
3. WHEN does a condition apply? When a new booking reservation is created.
4. WHY is this needed? For clearer visibility and for tracking equipment due dates more accurately.
5. HOW could we verify it? Log into the system, create a new booking reservation, save it, and then check the UI to verify that the specific return date was recorded correctly and is saved automatically within the system.

## 3. Requirements Surgery

### 1. "The system shall be user-friendly."
PROBLEM: It's too vague on what users are involved, what the system needs to do and what is "user-friendly" (subjective).

CLARIFICATION QUESTION: "What users are involved for this system? What does the system do?"

MISSING INFORMATION: The specific types of users included for this experience and the specific workflows that needs to become simplified for use.

### 2. "The system shall notify users about bookings."
PROBLEM: It's too vague on what users are involved, whether it's all users or a single user that gets the notifications, and what type of notifications would be given in relation to the bookings.

CLARIFICATION QUESTION: "What users are involved for this system? What types of notifications will the system use?"

MISSING INFORMATION: The recipient who actually gets the notifications, the method of delivering the notifications and the action that triggers the notification.

### 3. "The system shall allow staff to create, edit and delete bookings and send reminders."
PROBLEM: It's too vague on what type of staff is involved, and if the staff may be able to operate the system with all other things they need to do.

CLARIFICATION QUESTION: "What type of staff is involved, is it all of the staff or a specific staff that can utilise the system?"

MISSING INFORMATION: The specific staff that is assigned and gains access to the controls and whether reminders are sent automatically or manually by the specific staff.

REQUIREMENT: "The system shall allow only authorized staff to create, edit and delete bookings, and automatically sending automatic email reminders to borrowers."

## 4. Functional Requirements

### "The technician needs to know whether equipment is available before confirming a booking."
1. WHO? The technician needs this requirement.
2. WHAT? To confirm the availability of an equipment before confirming a booking.
3. WHEN? The booking would be confirmed once the availability of an equipment has been confirmed.
4. WHY? To avoid unnecessary bookings for out-of-stock equipment.
5. HOW? To verify, the system should consider the quantity of the equipment and the availability date for the equipment.

### FR-01 "The system shall allow an authorised user to view equipment availability for a selected date."
1. WHO? The authorised user needs this requirement.
2. WHAT? To be able to view information about the available equipment.
3. WHEN? Information will be revealed when the selected date is inputted into the system.
4. WHY? To verify if the equipment is available in stock before confirming a user's booking.
5. HOW? To verify, the system should display the correct remaining stock count for that specific day when the user selects an equipment and a date.

### FR-02 "The system shall prevent a user from booking a selected equipment that has already been booked or is out of stock for the selected dates."
1. WHO? The authorised user and the system needs this requirement.
2. WHAT? To be able to prevent and block user bookings from being recorded and saved.
3. WHEN? When the selected equipment has already been booked or is out of stock.
4. WHY? To prevent the case of double bookings and misleading users into believing the selected equipment is "available".
5. HOW? To verify, the system should check whether the selected is available or not, and if it's not, block the user, save nothing, and leave an error message to state the selected equipment has already been booked or is unavailable.

### FR-03 "The system shall require the user to input an expected return date before a new booking can be successfully saved."
1. WHO? The authorised user, the technician, and the system needs this requirement.
2. WHAT? To require an input of an expected return date.
3. WHEN? Before a new booking can be successfully saved into the database.
4. WHY? To make sure that technicians always know exactly when the equipment is being returned back, so it can prevent blank or missing return dates.
5. HOW? To verify, the system should block the new booking from being saved if the user attempts to save their booking without any return date inputted, where the system should then give a notification to the user to input an expected return date.

## 5. Quality Requirements
### NFR-01 "The system shall display equipment availability search results within 2 to 3 seconds of a user submitting their request."
1. WHO? The system and the staff could need this when the system is interacting with the user.
2. WHAT? To display equipment availability in real time.
3. WHEN? Within 2 to 3 seconds of the user submitting their requests.
4. WHY? To ensure that the system is fast, efficient and responsive so that the staff can quickly confirm the details for the user.
5. HOW? To verify, use an online or a physical stopwatch to measure the time it takes for the system to get the search results once the user presses the submission button/input to submit their request, and record and check the consistency of the time each test (between 2 to 3 seconds).

## 6. Project Application

## 7. Reflection
Upon the completion of Analysis/Specification phase, there is a clear difference between statements when it comes to identifying which statement can be confirmed as a problem (e.g. the camera statement) and a solution (e.g. the mobile app statement). There is also the fact of having vague terms could lead to massive confusion, no matter how good they sound (e.g. the user-friendly requirement is too vague as it doesn't specify on what users are involved and what action the system needs to do that is considered as "user-friendly", which is subjective). Therefore, it is important to utilise the WHO, WHAT, WHEN, WHY, and HOW questions to make the requirement more clearer and functional. Finally, the difference between functional requirements and non-functional requirements is that functional requirements are describing what the system needs to do, whereas non-functional requirements are describing how the system should perform.


