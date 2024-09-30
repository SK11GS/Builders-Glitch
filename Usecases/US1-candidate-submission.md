# Use case - Candidate resume submission

This use case is about allowing candidates to submit a resume, refine the resume, and generate an anonymized summary.

## Involved containers
<Container image goes here>

Involved containers:
- Resume Manager
- Resume / Job Enhancer
- Anonymizer

## Sequence diagram
![candidate-submission.jpg](images%2Fcandidate-submission.jpg)

### Sequence diagram description

A candidate uploads their resume through the Resume Manager module. 

The uploaded resume is then sent to the Resume AI module, which analyzes the content and offers helpful suggestions for improvement.

The candidate can choose to either accept the suggestions or make their own edits before resubmitting the resume. This process can be repeated until the candidate is satisfied with the final version.

The candidate can submit their resume to the Anonymizer once they are satisfied with the final version.

The Anonymizer will generate an anonymized resume for the resume and send it back to the Resume manager.
