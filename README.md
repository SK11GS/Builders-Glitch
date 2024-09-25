# Builders-Glitch

# 1. Candidate's Perspective:
## Registration & Profile Management
### Registration:
- Candidates register on the ClearView platform by providing basic demographic and contact information.
- The system sends a confirmation email, and candidates must verify their account.

### Profile Creation:
- Candidates create a profile by uploading a resume and completing additional required fields.
- AI within the ClearView platform analyzes the resume and provides resume improvement tips to align with job market demands and best practices (**hard requirement**).
- Candidates can either accept the AI-generated suggestions or manually modify their resume based on the recommendations.

### Anonymization of PII:
- The ClearView platform's AI anonymizes all personal identifiable information (PII) that may introduce bias, such as race, culture, or lifestyle characteristics (**hard requirement**).

## Job Matching & Interaction
### AI Job Matching:
- AI within the ClearView platform matches the anonymized resume to relevant job postings by comparing candidate experience and skill sets with job descriptions and generating a similarity score (**hard requirement**).
- For each job match, the AI generates a SMART goal representation of the candidate's experience specific to that role (**hard requirement**). These SMART goals emphasize Specific, Measurable, Achievable, Relevant, and Time-bound goals to make the candidate's qualifications clearer to hiring managers.

### Employer Interest:
- Candidates can view how many employers have expressed interest in their anonymized profile.

### Interact with Employers:
- Candidates can only contact employers who have unlocked their profile through the ClearView platform.

### Resume Update or Removal:
- **Mark Profile as Inactive:** Candidates can remove or update their resumes at any point.
- Candidates can mark their profile as "inactive" once hired, allowing hiring managers to avoid offering additional roles.

### Survey Submission:
- After completing an interview, candidates receive a 5-question survey to rate the interviewer and provide feedback on the process.

## Notifications
### Real-time Notifications:
- Candidates receive notifications when:
  - Hiring managers view their profile.
  - Employers unlock more detailed information (e.g., "Hiring Manager from XYZ viewed your profile for Operations Manager role in Portland, Oregon").

# 2. Hiring Manager's Perspective:
## Registration & Job Posting
### Registration:
- Employers or hiring managers register on the ClearView platform, with public data auto-filled and non-public data manually input (**hard requirement**).

### Create Job Postings:
- Employers upload job descriptions and relevant role requirements.

### Dashboard & Workspace:
- Hiring managers access a dashboard to manage job postings, view matched candidates, and perform administrative tasks.

## Candidate Matching & Interaction
### Receive Matching Candidates:
- AI within the ClearView platform matches candidates based on the posted job descriptions and generates a similarity score (**hard requirement**).
- The AI also generates SMART goal representations of each candidate’s experience according to the job requirements for easier comparison.

### Anonymized Candidate Profiles:
- Hiring managers view anonymized profiles, where all PII is removed to eliminate potential bias (**hard requirement**).

### Unlock Candidate Profiles:
- Hiring managers can unlock the full candidate profile (including anonymized details) after paying to proceed with the hiring process (**hard requirement**).

### Survey Submission Post Interview:
- Hiring managers complete a 5-question survey about candidates post-interview to evaluate the hiring process and provide feedback for recruitment strategy improvement.

## DEI Consultant Involvement
### DEI Consultant Inclusion:
- Hiring managers can include a DEI Consultant in the interview process to monitor for potential bias. This is offered as an additional service at a cost.
- The DEI Consultant observes interviews, records unconscious bias, and provides feedback to the ClearView Admin via the ClearView Platform.

## Status Updates & Interactions
### Update Role Status:
- Hiring managers can update job status as "Open," "Interviewing," "Offer Extended," "Accepted," or "Hired."

### Notifications:
- Hiring managers are notified when:
  - A new match for their posted role is available. This can be consolidated into a single message across all job postings and redirect the hiring manager to the dashboard.
  - Candidates are notified when hiring managers express interest or unlock their profile.

## Invoicing & Payments
### Payment for Profile Unlocks:
- Hiring managers must pay to unlock the candidate’s profile to view detailed information and proceed with the hiring process.

# 3. ClearView Platform Administrator's Perspective:
## Platform Maintenance & Oversight
### Data Anonymization:
- The ClearView platform ensures that all candidate PII is anonymized to reduce bias in the recruitment process.

### Match Notification Management:
- Admins oversee notifications sent to all relevant parties (candidates, hiring managers, admins) when a match is made.

## Bias Reporting & Data Management
### Unconscious Bias Reporting:
- DEI Consultants submit their findings on unconscious bias observed during interviews to the ClearView Admin.
- The ClearView Admin compiles these findings into unconscious bias reports for executive management.

### Generate Bias Reports:
- Admins generate comprehensive reports based on DEI Consultant feedback, detailing any unconscious bias observed during the interview process.
- These reports are shared with executive management to help address and mitigate bias in hiring decisions.

### Propose Strategic Bias Reduction:
- Based on the bias reports, ClearView Admin provides actionable recommendations to hiring managers and executives to help reduce bias and improve fairness in interviews.

## Hiring Manager Interaction
### Profile Viewing Permissions:
- Admins ensure that hiring managers can only unlock and view candidate profiles after they have matched with a job posting and paid to unlock the profile.

### Scheduling Interviews:
- Admins ensure that hiring managers have access to interview scheduling features within the ClearView platform once a candidate's profile is unlocked.

### Candidate Status Management:
- Admins ensure that hiring managers can update a candidate’s application status to "Interviewing," "Offer Issued," "Accepted," or "Rejected."

### Status Updates:
- Any changes to a candidate’s status (e.g., hired, rejected, accepted, or interviewing) are reflected across the platform, ensuring transparency for candidates and hiring managers.

## Data Collection & Reporting
### Maintain Demographic Data:
- Admins ensure that detailed demographic data is collected and maintained for all candidates, tracking those who are hired or rejected.

### Reporting & Analytics:
- Admins generate and maintain monthly KPI reports related to hiring, interview processes, and any hiring disparities. These reports include:
  - Demographics of candidates at various stages.
  - Number of candidates matched, interviewed, and hired/rejected.
  - Disparities in hiring based on demographic factors.

### Data Aggregation:
- The platform aggregates data points, tracking how many candidates reach various stages in the process (interview, offer, rejection).

### Internal Data Management:
- Admins maintain an internal system to track user behaviors, hiring patterns, and candidate success rates.

## Notifications & Communication
### Three-way Notifications:
- Admins ensure that notifications about matches, interview schedules, and status updates are shared among candidates, hiring managers, and ClearView admins to keep everyone informed.

## Bias Monitoring & Management
### Bias Monitoring:
- Admins monitor system-level data to ensure that bias-reduction mechanisms (such as resume anonymization) are functioning correctly.

### Ensure Fair Matches:
- Admins validate that AI-driven matching is fair and aligned with diversity and inclusion goals.

# 4. DEI Consultant’s Perspective:
## Bias Monitoring
### Shadow Interviews:
- DEI Consultants shadow live interviews at the request of the hiring manager to monitor for potential unconscious bias.
- DEI Consultants record instances of potential bias observed during interviews.

### Record Unconscious Bias:
- DEI Consultants document any instances of unconscious bias, such as biased language or behavior, during the interview process.

### Submit Findings to Admin:
- After observing interviews, DEI Consultants submit their findings on unconscious bias to the ClearView Admin for further analysis.

## Reporting & Feedback
### Provide Reports to Executive Management:
- ClearView Admin compiles the unconscious bias reports submitted by DEI Consultants and shares them with the hiring company’s executive management.

### Propose Bias Reduction Strategies:
- DEI Consultants and ClearView Admins may propose bias-reduction strategies based on the reports, which can be used by executive management to address and mitigate bias in future interviews.

# 5. Technical & Integration Requirements:
## AI-Driven Features within ClearView Platform
### SMART Goal Conversion:
- The **AI integrated within the ClearView platform** converts candidate resumes into SMART goals (Specific, Measurable, Achievable, Relevant, Time-bound) based on each matched job (**hard requirement**).

### AI Job Matching:
- The AI matches candidates to jobs based on the SMART goal representation and generates a similarity score to assess how well candidates meet the job requirements (**hard requirement**).

### AI Resume Suggestions:
- The AI provides resume improvement tips, which candidates can either accept or manually modify to refine their profiles.

## Reporting & Analytics
### Reports & Analytics:
- Analytics and reports are available to all users with appropriate access levels, allowing them to track:
  - Candidate matches and job postings.
  - Hiring patterns and demographic insights.
  - Bias detection in interview and hiring processes.

### Unconscious Bias Reports:
- ClearView Admin generates reports based on DEI Consultant findings and shares them with executive management to address unconscious bias in interviews.

## HR System Integration
### HR System Integration:
- The platform integrates with popular HR systems (e.g., SAP SuccessFactors, UKG Pro, Workday) for seamless synchronization of job postings, candidate information, and reporting data.
