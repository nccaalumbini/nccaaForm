1. Project Objective

The goal of this project is to create an easy-to-use online platform where NCC cadets can submit their personal and training information through a web-based form. The system will then automatically generate a standardized form document for each cadet and store it securely in Google Drive.

Key Objectives:

Simplify the data submission process for NCC cadets.

Automatically generate formal forms/documents from submitted data.

Maintain organized storage of forms in Google Drive.

Support Nepali language for form fields and outputs.

2. Current Implementation

Technologies Used: HTML, CSS, JavaScript.

User Workflow:

Cadet accesses the web form.

Cadet fills in personal and training details.

On submission, the system is supposed to generate a formal document (form) for the cadet.

Generated form is intended to be stored in a dedicated folder in Google Drive.

Functional Highlights:

Simple and responsive web form.

User-friendly interface designed for cadets.

Logic implemented to capture form inputs and trigger form generation.

3. Issues / Current Challenges

The system is currently unable to generate the final form in Nepali.

Form generation logic works partially but does not produce the finalized document.

Integration with Google Drive for storage is pending/facing errors.

Some errors observed in JavaScript related to handling Nepali characters and formatting.

4. Proposed Next Steps / Solutions

Nepali Language Support:

Implement Unicode support to correctly display and save Nepali text in forms.

Form Generation:

Use libraries like jsPDF or Google Docs API to generate PDFs in Nepali.

Google Drive Integration:

Ensure proper API authentication and folder setup for storing cadet forms.

Testing & Validation:

Test the entire workflow with sample cadet data.

Validate that forms are correctly generated, named, and stored.

UI/UX Enhancements:

Refine form layout, improve responsiveness, and handle validation messages clearly.

5. Conclusion

The NCC Cadet Form Automation System is designed to simplify data submission and record keeping for cadets. While the form input and user interface are functional, the PDF generation in Nepali and automated storage in Drive remain pending. Completing these tasks will fully automate the workflow, reduce manual errors, and provide a professional, standardized record for each cadet.
