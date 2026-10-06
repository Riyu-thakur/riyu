# MASTER PROMPT — BUILD COMPLETE FULL-STACK MCQ WEBSITE

You are the MAIN AGENT and Lead Full-Stack Architect. Your task is to plan, develop, test, secure, and deliver a complete production-ready MCQ-based learning and examination website named:

# MCQ Based

The application must be a modern, responsive, fast, scalable full-stack MCQ platform.

Do not create only a UI prototype. Build the complete working application with frontend, backend/database integration, authentication, role-based access, test engine, result system, admin management, validation, security, responsive design, loading states, error handling, and deployment-ready code.

---

# 1. TECHNOLOGY STACK

## Frontend
Use:

- React.js
- Vite
- JavaScript/JSX
- React Router
- CSS or a well-structured CSS architecture
- Responsive design
- Reusable components
- Context API or another lightweight state-management approach

Do not use unnecessary libraries when native React/CSS is sufficient.

## Backend / Database
Use Firebase:

- Firebase Authentication
- Cloud Firestore
- Firebase Storage where required
- Firebase Security Rules
- Firebase Cloud Functions only where genuinely required

Use Firebase as the primary backend/database.

## Deployment
The project must be deployment-ready for:

- Firebase Hosting
or
- Vercel / Netlify for frontend

The application must work with Firebase in production.

---

# 2. DESIGN THEME

Use a premium:

# AQUA THEME

The entire website should have an aqua/blue/white modern educational dashboard style.

Design goals:

- Clean
- Professional
- Modern
- Premium
- Student-friendly
- Mobile responsive
- Smooth animations
- Excellent typography
- Good spacing
- Card-based UI
- Rounded corners
- Subtle shadows
- Aqua gradients
- Accessible contrast

Primary visual direction:

- Aqua
- Cyan
- Sky blue
- White
- Dark navy for important text

Do not make the website excessively colorful.

Create a consistent design system for:

- Buttons
- Cards
- Inputs
- Tabs
- Modals
- Tables
- Badges
- Alerts
- Progress bars
- Test questions
- Navigation
- Admin dashboard

Support both desktop and mobile screens.

---

# 3. MULTI-AGENT DEVELOPMENT SYSTEM

You are the MAIN AGENT.

You must divide the development into specialized SUB AGENTS.

Create and manage the following sub-agents:

## SUB AGENT 1 — UI/UX Architect

Responsibilities:

- Design complete application layout
- Aqua theme
- Responsive design
- Design system
- Components
- User navigation
- Admin navigation
- Mobile navigation
- Empty states
- Loading states
- Error states
- Accessibility
- UX consistency

Deliver:

- UI architecture
- Page layouts
- Component requirements
- Responsive behavior

---

## SUB AGENT 2 — React Frontend Developer

Responsibilities:

- Build React application
- React Router
- Components
- Pages
- Forms
- Test interface
- User dashboard
- Admin dashboard
- Search
- Filters
- Pagination
- Notifications
- Protected routes

All components must be reusable.

---

## SUB AGENT 3 — Firebase Backend Developer

Responsibilities:

- Firebase initialization
- Authentication
- Firestore database
- Storage
- Security rules
- Role management
- CRUD operations
- Query optimization
- Firebase configuration
- Backend validation

Create a clean service layer so React components do not directly contain unnecessary Firebase logic.

---

## SUB AGENT 4 — MCQ/Test Engine Developer

Responsibilities:

Build the complete examination engine.

Features:

- Question display
- Multiple-choice options
- Single correct answer
- Question navigation
- Previous/Next
- Question palette
- Answer state
- Mark for review
- Timer
- Auto submit
- Manual submit
- Confirmation before submit
- Prevent accidental test loss
- Score calculation
- Correct/incorrect answer evaluation
- Percentage
- Accuracy
- Attempt statistics
- Result generation
- Test history

---

## SUB AGENT 5 — Admin Panel Developer

Responsibilities:

Create a complete Admin Panel.

Admin must be able to manage:

- Categories
- Subjects
- Topics
- Tests
- Questions
- Options
- Correct answers
- Explanations
- Users
- User roles
- Test attempts
- Results
- Reports
- Announcements
- Website settings

Include CRUD operations.

---

## SUB AGENT 6 — Security Engineer

Responsibilities:

- Firebase Security Rules
- Authentication authorization
- Admin role protection
- User role protection
- Database access restrictions
- Input validation
- Prevent unauthorized test/question modification
- Prevent unauthorized result modification
- Secure admin routes
- Secure Firebase Storage
- Basic abuse prevention

Never expose sensitive admin operations to normal users.

---

## SUB AGENT 7 — QA/Test Engineer

Responsibilities:

Test:

- Authentication
- Registration
- Login
- Logout
- Password reset
- Category navigation
- Topic navigation
- Test start
- Test timer
- Answer selection
- Question navigation
- Test submission
- Result calculation
- Result history
- Admin CRUD
- Search
- Filters
- Mobile responsiveness
- Error handling
- Firebase integration
- Security rules

Find and fix bugs before final delivery.

---

## SUB AGENT 8 — Performance/Deployment Engineer

Responsibilities:

- Optimize React rendering
- Lazy-load routes where useful
- Optimize Firebase queries
- Avoid unnecessary reads/writes
- Optimize images/assets
- Production build
- Environment configuration
- Firebase hosting configuration
- Deployment instructions

---

# 4. MAIN AGENT RESPONSIBILITY

As MAIN AGENT:

1. Create the complete architecture.
2. Delegate tasks to sub-agents.
3. Keep all sub-agents aligned with a single database schema and design system.
4. Integrate all modules.
5. Resolve conflicts between agents.
6. Run final tests.
7. Fix broken functionality.
8. Ensure the application works end-to-end.
9. Do not stop after creating individual pages.
10. Deliver one integrated working website.

---

# 5. WEBSITE INFORMATION ARCHITECTURE

The website should follow this basic user journey:

HOME PAGE
↓
CATEGORIES
↓
SELECT CATEGORY
↓
TOPICS / TEST LIST
↓
SELECT TEST
↓
TEST INSTRUCTIONS
↓
START TEST
↓
MCQ TEST ENGINE
↓
SUBMIT TEST
↓
RESULT PAGE
↓
DETAILED RESULT
↓
TEST HISTORY / PERFORMANCE

---

# 6. HOME PAGE

Create an attractive homepage.

Include:

## Header

- Logo: MCQ Based
- Home
- Categories
- Tests
- About
- Contact
- Search
- Login
- Register

After login:

- Dashboard
- Profile
- My Tests
- Results
- Logout

If admin is logged in:

- Admin Dashboard

## Hero Section

Example concept:

"Prepare Smarter. Practice Better. Score Higher."

Include:

- Start Practice button
- Browse Categories button
- Search tests

## Statistics

Show dynamic statistics from Firebase:

- Total Categories
- Total Tests
- Total Questions
- Total Students

## Categories Section

This is extremely important.

Display many categories as cards.

Example:

- General Knowledge
- Computer
- Programming
- HTML
- CSS
- JavaScript
- React
- Python
- C
- C++
- Java
- SQL
- Networking
- Operating System
- DBMS
- Cyber Security
- Aptitude
- Reasoning
- Mathematics
- Science
- English
- Current Affairs
- Government Exams
- Railway
- SSC
- Banking
- NDA
- Other Exams

Categories must come dynamically from Firestore.

The admin must be able to add/edit/delete categories.

---

# 7. CATEGORY PAGE

When the user clicks any category:

Open a dedicated category page.

Example:

Category:
"Computer"

Display:

- Category title
- Description
- Total tests
- Total questions
- Search
- Sort
- Filter

Then show multiple tests/topics.

Example:

Computer
--------------------------------
HTML MCQ Test 1
HTML MCQ Test 2
HTML MCQ Test 3
CSS Basic Test
CSS Advanced Test
JavaScript Test 1
JavaScript Test 2
Computer Fundamentals
Internet & Networking
--------------------------------

Each test card must show:

- Test title
- Number of questions
- Difficulty
- Duration
- Attempt count
- Description
- Start Test button

---

# 8. TEST DETAILS PAGE

Before starting a test, show:

- Test title
- Category
- Topic
- Number of questions
- Duration
- Difficulty
- Instructions
- Passing percentage
- Negative marking if enabled
- Maximum marks

Buttons:

- Start Test
- Back

Show a confirmation dialog before starting.

---

# 9. TEST ENGINE

Create a professional examination interface.

Desktop:

Left/center:
Question area

Right:
Question palette / test summary

Mobile:

Question area on top
Navigation controls
Question palette in collapsible drawer/modal

Each MCQ should have:

Question number

Question text

Optional question image

Four options:

A
B
C
D

Allow future support for:

- 2 options
- 3 options
- 4 options
- 5 options

Each question can optionally contain:

- Explanation
- Image
- Code snippet

---

# 10. TEST CONTROLS

Include:

- Previous
- Next
- Save & Next
- Mark for Review
- Clear Answer
- Submit Test

Question palette states:

- Not visited
- Answered
- Not answered
- Marked for review
- Answered + marked

Use clear visual indicators.

---

# 11. TIMER

Implement a reliable countdown timer.

Example:

60:00

When time reaches zero:

Automatically submit the test.

Show warning states when time is low.

The timer must not reset unexpectedly during navigation or page re-rendering.

---

# 12. TEST SUBMISSION

Before manual submission:

Show confirmation:

"Are you sure you want to submit this test?"

Display:

- Attempted questions
- Unattempted questions
- Marked questions
- Remaining time

After submission:

- Lock the attempt
- Calculate result
- Save result to Firebase
- Redirect to Result Page

Do not allow users to modify a completed attempt.

---

# 13. RESULT PAGE

Create a professional result dashboard.

Show:

- Score
- Maximum marks
- Percentage
- Correct answers
- Incorrect answers
- Unanswered
- Accuracy
- Time taken
- Total time
- Pass/Fail
- Rank if implemented

Use charts/progress visualization where useful.

Buttons:

- Review Answers
- Try Again
- Back to Tests
- View History

---

# 14. ANSWER REVIEW PAGE

After a test, users can review:

Question

Selected answer

Correct answer

Result:

- Correct
- Incorrect
- Not attempted

Show explanation when available.

Important:

The user should not be able to change answers from the review page.

---

# 15. USER AUTHENTICATION

Use Firebase Authentication.

Support:

- Register
- Login
- Logout
- Forgot Password
- Password Reset
- Email-based authentication

Optionally support Google login if easy to implement.

Registration fields:

- Full Name
- Email
- Password
- Confirm Password

User profile:

- Name
- Email
- Profile photo
- Created date
- Role
- Statistics

Default role:

"user"

Admin role:

"admin"

Do not allow users to assign themselves the admin role.

---

# 16. USER DASHBOARD

Create:

# Student Dashboard

Show:

- Welcome message
- Total attempts
- Completed tests
- Average score
- Average percentage
- Best score
- Recent tests
- Category performance
- Progress
- Recommended tests

Dashboard cards:

Total Attempts
Average Score
Best Score
Tests Completed

Recent attempts table:

- Test
- Category
- Score
- Percentage
- Date
- View Result

---

# 17. USER PROFILE

Create Profile Page.

Allow:

- Edit name
- Profile photo
- Change password through Firebase
- View account information

Display:

- Name
- Email
- Join date
- Total tests
- Average score

---

# 18. TEST HISTORY

Create:

# My Test History

Show:

- Test name
- Category
- Date
- Score
- Percentage
- Status
- View Result

Include:

- Search
- Filter by category
- Sort by date
- Pagination

---

# 19. SEARCH SYSTEM

Global search should find:

- Categories
- Tests
- Topics

Search should be fast and user-friendly.

Create search suggestions where practical.

---

# 20. ADMIN PANEL

Create separate protected admin application area.

Admin Dashboard should show:

- Total Users
- Total Categories
- Total Tests
- Total Questions
- Total Attempts
- Average Score

Also show recent activity.

---

# 21. ADMIN CATEGORY MANAGEMENT

Admin can:

- Create category
- Edit category
- Delete category
- Activate/deactivate category
- Add description
- Add icon/image
- Set display order

Fields:

- Name
- Slug
- Description
- Image/Icon
- Status
- CreatedAt
- UpdatedAt

Prevent deleting a category if dependent data exists unless proper cascading behavior is implemented.

---

# 22. ADMIN TOPIC/TEST MANAGEMENT

Admin can:

- Create test
- Edit test
- Delete test
- Publish/unpublish test
- Duplicate test
- Set category
- Set topic
- Set difficulty
- Set duration
- Set number of questions
- Set marks
- Set passing percentage
- Enable/disable negative marking

Example:

Test:
JavaScript Basics

Category:
Programming

Topic:
JavaScript

Difficulty:
Easy

Questions:
20

Duration:
15 minutes

Passing:
40%

Negative Marking:
0.25

---

# 23. ADMIN QUESTION MANAGEMENT

Admin must have complete question management.

Create question form:

- Select category
- Select test
- Question text
- Option A
- Option B
- Option C
- Option D
- Correct answer
- Explanation
- Difficulty
- Question image
- Status

Actions:

- Add
- Edit
- Delete
- Duplicate
- Publish
- Unpublish

Add validation so a question cannot be published without a valid correct answer.

---

# 24. QUESTION BULK IMPORT

Implement a practical question import system.

Support CSV import.

CSV example:

question,optionA,optionB,optionC,optionD,correctAnswer,explanation,difficulty

Allow admin to:

- Upload CSV
- Preview questions
- Validate rows
- Show errors
- Import valid questions
- Cancel import

Do not blindly insert invalid records.

---

# 25. ADMIN USER MANAGEMENT

Admin can view users.

Display:

- Name
- Email
- Role
- Status
- Created Date
- Attempts

Admin can:

- Search users
- Filter users
- Disable/enable account where architecture permits
- Change role through a secure admin-only mechanism
- View user attempts
- View user performance

Do not permit a normal user to modify their own role.

---

# 26. ADMIN RESULT MANAGEMENT

Admin can view all test attempts.

Display:

- User
- Test
- Category
- Score
- Percentage
- Time taken
- Date

Include:

- Search
- Filters
- Date filters
- Category filter
- Test filter
- User filter

---

# 27. ADMIN ANALYTICS

Create useful analytics.

Show:

- Tests attempted over time
- Daily attempts
- Popular categories
- Average scores
- Top-performing tests
- Difficult questions
- Most attempted questions

Use Firebase aggregation/query strategies efficiently.

Do not perform wasteful reads.

---

# 28. LEADERBOARD

Implement optional leaderboard functionality.

Show:

- Rank
- User
- Tests completed
- Score/points
- Percentage

Provide filters by:

- All time
- Monthly
- Weekly

Ensure privacy-sensitive information is not exposed.

---

# 29. FAVORITES / BOOKMARKS

Logged-in users can save:

- Favorite tests
- Bookmark questions where architecture supports it

Create:

# My Favorites

---

# 30. NOTIFICATIONS

Create notification infrastructure.

Types:

- New test added
- Important announcement
- Test result
- System notification

Admin should be able to create announcements.

---

# 31. ABOUT PAGE

Create:

# About MCQ Based

Explain:

- What the platform provides
- Practice tests
- Exam preparation
- Categories
- Performance tracking

---

# 32. CONTACT PAGE

Create contact form.

Fields:

- Name
- Email
- Subject
- Message

Validate fields.

Store submissions securely in Firebase.

Admin should be able to view contact submissions.

---

# 33. FAQ PAGE

Create FAQ section covering:

- How to create an account
- How to start a test
- How scoring works
- How results are saved
- How to review answers
- How to reset password
- Other common questions

---

# 34. ERROR / UTILITY PAGES

Create:

- 404 Not Found
- Unauthorized
- Access Denied
- Loading Page
- Network Error
- Empty State
- Firebase Error State

---

# 35. ROUTING STRUCTURE

Suggested route architecture:

/
/categories
/category/:categoryId
/test/:testId
/test/:testId/instructions
/test/:testId/start
/test/:testId/result/:attemptId
/test/:testId/review/:attemptId

/login
/register
/forgot-password

/dashboard
/profile
/history
/favorites
/leaderboard
/notifications

/about
/contact
/faq

/admin
/admin/dashboard
/admin/categories
/admin/topics
/admin/tests
/admin/questions
/admin/users
/admin/attempts
/admin/analytics
/admin/announcements
/admin/contact-messages
/admin/settings

Protect routes based on authentication and role.

---

# 36. FIRESTORE DATABASE ARCHITECTURE

Use a clean scalable schema.

Suggested collections:

users
categories
topics
tests
questions
attempts
answers
favorites
notifications
announcements
contactMessages
settings

Suggested user document:

users/{userId}

Fields:

uid
name
email
photoURL
role
status
createdAt
updatedAt

Suggested category:

categories/{categoryId}

Fields:

name
slug
description
image
icon
status
displayOrder
createdAt
updatedAt

Suggested test:

tests/{testId}

Fields:

title
slug
categoryId
topicId
description
instructions
difficulty
durationMinutes
questionCount
marksPerQuestion
passingPercentage
negativeMarking
isPublished
createdAt
updatedAt

Suggested question:

questions/{questionId}

Fields:

testId
categoryId
topicId
questionText
imageURL
options
correctAnswer
explanation
difficulty
status
createdAt
updatedAt

Options can be stored in structured form.

Suggested attempt:

attempts/{attemptId}

Fields:

userId
testId
categoryId
answers
score
totalMarks
percentage
correctCount
incorrectCount
unansweredCount
accuracy
timeTaken
submittedAt
status

Do not store unnecessary sensitive information.

---

# 37. FIRESTORE SECURITY

Create proper Firebase Security Rules.

Rules must ensure:

Public users:
- Can read published categories/tests as required.

Authenticated users:
- Can read published tests/questions.
- Can create their own attempts.
- Can read only their own private attempt/result data.
- Can modify only permitted personal profile fields.

Admin:
- Full authorized CRUD access.

Never trust frontend role checks alone.

Security must be enforced in Firebase Rules.

---

# 38. TEST RANDOMIZATION

Support optional test randomization:

- Random question order
- Random option order

The final result must still use the correct answer securely.

Ensure answer validation cannot be manipulated through client-side logic.

---

# 39. MCQ SCORING

Implement configurable scoring.

Example:

Correct:
+1

Incorrect:
0

Or:

Correct:
+1

Incorrect:
-0.25

Unanswered:
0

The score system must use test configuration.

Never hard-code one scoring model globally.

---

# 40. RESPONSIVENESS

The website must work correctly on:

- Desktop
- Laptop
- Tablet
- Android phone
- iPhone

Important mobile pages:

- Home
- Category
- Test list
- Test engine
- Result
- Dashboard
- Admin panel

The exam interface must be especially optimized for mobile.

---

# 41. ACCESSIBILITY

Implement:

- Semantic HTML
- Keyboard navigation
- Proper labels
- Accessible buttons
- Focus states
- Alt text
- Sufficient contrast
- Error messages
- Screen-reader-friendly controls where practical

---

# 42. PERFORMANCE

Optimize:

- Firebase reads
- React re-renders
- Images
- Route loading
- Queries
- Pagination
- Firestore indexes where necessary

Avoid retrieving an entire collection when only a limited result set is needed.

Use pagination/limits.

---

# 43. LOADING & ERROR UX

Every asynchronous operation needs proper UI.

Examples:

- Skeleton loading
- Spinner
- Saving state
- Submit state
- Empty result state
- Firebase error notification
- Network error
- Retry option

Never leave the user staring at a blank screen.

---

# 44. CODE QUALITY

Use:

- Reusable components
- Clean folder architecture
- Separate Firebase services
- Utility functions
- Constants
- Custom hooks where useful
- Centralized error handling
- Environment variables
- Clear naming
- Comments only where useful

Avoid:

- Huge single components
- Duplicate code
- Hard-coded data
- Hard-coded admin credentials
- Firebase keys committed improperly
- Repeating Firebase logic everywhere

---

# 45. SUGGESTED PROJECT STRUCTURE

Create a scalable structure similar to:

src/
  components/
  pages/
    public/
    auth/
    user/
    admin/
  layouts/
  routes/
  services/
    firebase/
  hooks/
  context/
  utils/
  constants/
  assets/
  styles/

Also maintain:

firebase/
  firestore.rules
  firestore.indexes.json
  storage.rules

root files:

- package.json
- vite.config.js
- .env.example
- README.md

---

# 46. SAMPLE INITIAL CATEGORIES

Seed development data with multiple categories so the homepage does not look empty.

Examples:

General Knowledge
Computer Fundamentals
HTML
CSS
JavaScript
React JS
Python
C Programming
C++
Java
SQL
DBMS
Networking
Operating System
Cyber Security
Aptitude
Reasoning
Mathematics
English
Science
Current Affairs
SSC
Railway
Banking
NDA

Create sample tests under several categories.

Each sample test should contain multiple MCQs so the complete test flow can be demonstrated.

---

# 47. ADMIN INITIALIZATION

Do not expose an admin signup option publicly.

Create a safe method for creating the first administrator, such as:

- Manual Firebase user creation
- Secure environment/config process
- Firebase Admin SDK / Cloud Function where appropriate

Document the procedure in README.

---

# 48. WEBSITE FOOTER

Footer should include:

MCQ Based

Links:

- Home
- Categories
- About
- Contact
- FAQ
- Privacy Policy
- Terms & Conditions

Also show:

© current year MCQ Based

---

# 49. PRIVACY AND TERMS PAGES

Create basic:

- Privacy Policy
- Terms & Conditions

Avoid making unsupported legal claims. Keep them as general application terms suitable for customization.

---

# 50. ADMIN SETTINGS

Create settings section.

Possible settings:

- Website name
- Website logo
- Website description
- Contact email
- Maintenance mode
- Default test duration
- Default passing percentage
- Leaderboard enable/disable

---

# 51. DATA VALIDATION

Validate:

- Email
- Password
- Required fields
- Question options
- Correct answer
- Test duration
- Percentage
- Negative marking
- Category relationships

Show user-friendly validation messages.

---

# 52. SECURITY REQUIREMENTS FOR TESTS

Do not expose unnecessary sensitive test data.

Important:

Never treat the React client as a trusted environment.

The frontend must not be the sole authority for:

- User roles
- Final score
- Admin permissions
- Result ownership

Use Firebase rules and secure backend logic where needed.

---

# 53. UX DETAILS

Add polished interactions:

- Hover effects
- Smooth transitions
- Button loading states
- Toast messages
- Confirmation modals
- Breadcrumbs
- Search/filter controls
- Pagination
- Sticky test timer where appropriate
- Sticky navigation
- Progress indicators

Do not overuse animations.

---

# 54. HOME PAGE CATEGORY EXPERIENCE

This is a core requirement.

The homepage must feel like a large MCQ library.

Example visual structure:

MCQ Based
------------------------------------------------
Search "Search MCQ, Test, Category..."
------------------------------------------------

Popular Categories

[ Computer ] [ HTML ] [ CSS ] [ JavaScript ]
[ Python ] [ Reasoning ] [ Aptitude ] [ GK ]
[ Science ] [ English ] [ Railway ] [ SSC ]
[ NDA ] [ Banking ] [ Networking ] [ SQL ]
...

When user clicks:

[JavaScript]

Open:

JavaScript
-------------------------------------
JavaScript Basics
JavaScript Variables
JavaScript Operators
JavaScript Functions
JavaScript Loops
JavaScript DOM
JavaScript ES6
JavaScript Advanced
-------------------------------------

When the user selects:

JavaScript Loops

Open:

Test Details

Then:

Start Test

Then:

MCQ Exam Interface

Then:

Result

Then:

Answer Review

This exact user journey must work.

---

# 55. ADMIN WORKFLOW

Admin workflow:

Login
↓
Admin Dashboard
↓
Create Category
↓
Create Topic
↓
Create Test
↓
Add Questions
↓
Publish Test
↓
Students can see it
↓
Students attempt test
↓
Results saved
↓
Admin sees analytics

Make this complete workflow functional.

---

# 56. DEVELOPMENT PROCESS

Follow this development sequence:

PHASE 1
Architecture + database schema + UI design system

PHASE 2
React project setup + Firebase configuration

PHASE 3
Authentication

PHASE 4
Public pages

PHASE 5
Category/topic/test system

PHASE 6
MCQ engine

PHASE 7
Result system

PHASE 8
User dashboard/history/profile

PHASE 9
Admin panel

PHASE 10
Analytics/leaderboard/favorites/notifications

PHASE 11
Security rules

PHASE 12
Testing and bug fixing

PHASE 13
Production optimization

PHASE 14
Deployment documentation

Do not move to the next phase while the previous critical functionality is broken.

---

# 57. AGENT COORDINATION RULE

The MAIN AGENT must maintain a shared specification.

Before coding a dependent module:

- Check existing architecture.
- Check existing database schema.
- Check existing route names.
- Check existing component names.
- Reuse existing components.
- Do not create duplicate systems.

If a sub-agent identifies an architectural issue, report it to the MAIN AGENT and resolve it centrally.

---

# 58. FINAL QUALITY CHECK

Before declaring the project complete, verify:

Authentication works.

Registration works.

Login works.

Logout works.

Password reset works.

Home page loads.

Categories load from Firebase.

Category navigation works.

Topics/tests load correctly.

Test details work.

Test starts correctly.

Timer works.

Questions work.

Options work.

Previous/Next works.

Mark for review works.

Clear answer works.

Question palette works.

Submit confirmation works.

Auto-submit works.

Scoring works.

Negative marking works if enabled.

Results save correctly.

Review answers works.

History works.

Profile works.

Favorites works if implemented.

Leaderboard works if implemented.

Admin login works.

Admin routes are protected.

Admin category CRUD works.

Admin test CRUD works.

Admin question CRUD works.

CSV question import works.

User management works.

Result management works.

Analytics work.

Contact form works.

Notifications/announcements work where implemented.

404 page works.

Mobile layout works.

Firebase Security Rules are implemented.

Production build succeeds.

No major console errors remain.

No broken links remain.

No hard-coded fake functionality remains.

---

# 59. FINAL DELIVERABLE

The MAIN AGENT must provide:

1. Complete React source code.
2. Firebase integration.
3. Firestore database schema.
4. Firestore security rules.
5. Firebase Storage rules if used.
6. Firestore indexes if required.
7. Sample/seed data.
8. Admin setup instructions.
9. Environment variable example.
10. Installation instructions.
11. Local development instructions.
12. Firebase deployment instructions.
13. Production build instructions.
14. Testing checklist.
15. Clear project folder structure.

The final application must be a real working:

# MCQ Based

full-stack MCQ examination and learning platform.

Do not deliver a static mockup.

Every major button and workflow must perform its intended function.

Build the system so additional categories, tests, questions, users, and features can be added later without redesigning the entire application.

Start by creating the architecture, database model, route map, component map, and task breakdown for all sub-agents. Then implement the application phase by phase and integrate everything into one production-ready system.
