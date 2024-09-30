# Use case - Hiring manager job requisition submission

This use case is about allowing hiring managers to submit and refine a job requisition before submitting it to the Match AI.

## Involved containers
<Container image goes here>

Involved containers:
- Job Manager
- Resume / Job Enhancer
- Talent Bridge

## Sequence diagram
![hiringmanager-submission.jpg](images%2Fhiringmanager-submission.jpg)

### Sequence diagram description

A hiring manager submits their job request through the Job Manager module. 

The uploaded job request is then sent to the Resume / Job Enhancer module, which analyzes the content and offers helpful suggestions for improvement.

The hiring manager can choose to either accept the suggestions or make their own edits before resubmitting the job request. This process can be repeated until the hiring manager is satisfied with the final version.

The hiring manager can submit their job request to the Match AI once they are satisfied with the final version.