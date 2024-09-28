# Use case - Hiring manager job match

This use case enables hiring managers to view an anonymized resume summary, purchase access to unlock the full resume, and export it to their external HR systems.

## Involved containers
<Container image goes here>

Involved containers:
- Match AI
- Notification Queue
- Job / Resume Manager
- Invoice
- External Integration
- Survey Manager

## Sequence diagram
![job-match.jpg](images%2Fjob-match.jpg)

### Sequence diagram description

The hiring manager is notified of a potential match for a job requisition they posted.

Upon receiving the notification, the hiring manager reviews the anonymized resume summary and decides whether to unlock the full resume.

If they choose to unlock the resume, a payment is made, granting access to the candidate's complete resume.

Should the hiring manager wish to proceed with an interview, they can export the resume to their external HR systems.

The hiring manager is presented with a survey which will allow us to improve the system.