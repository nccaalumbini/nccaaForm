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

Proposed System Update: Database-Driven Form Generation
1. Current Limitation

Currently, the system aims to save each cadet’s form as a file in Google Drive. This has some challenges:

Manual management of files becomes cumbersome as the number of cadets grows.

Searching or retrieving a specific cadet’s form requires navigating Drive folders.

Integration and automation with Drive APIs can be error-prone.

2. Proposed Solution

Instead of saving generated forms directly to Drive, we can:

Store cadet data in a database (e.g., MySQL, PostgreSQL).

Generate forms on-demand:

When needed, the system fetches a cadet’s data from the database.

Generates a formal PDF form dynamically (e.g., using jsPDF or PHP libraries like TCPDF).

Print or download:

Users/admins can directly print the form or download it as a PDF without storing multiple static files.

3. Advantages

Centralized storage: All cadet data is stored in one place (the database).

Easy search and retrieval: Forms can be generated for any cadet instantly.

Reduced storage needs: No need to maintain separate files for each submission.

Better scalability: Works for hundreds or thousands of cadets without clutter.

Dynamic updates: If cadet data changes, the latest form is generated every time.

Professional workflow: Aligns with modern data management best practices.

4. Implementation Outline

Database Design:

Table cadets with columns: id, name, dob, province, district, training_details, contact_info, etc.

Form Generation:

Fetch data using a query like SELECT * FROM cadets WHERE id = ?.

Fill the form template dynamically.

Export as PDF using jsPDF (front-end) or TCPDF / FPDF (back-end).

Optional: Add a web interface where admins can search cadets and generate/download their forms
