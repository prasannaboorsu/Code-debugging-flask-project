# Note Taking Application Bug Fix Report

## Bug 1: Template Not Found Error
- **Description:** The Flask application was unable to locate the HTML template file.
- **Approach:** Moved the `home.html` file to the `templates` directory to ensure Flask can locate it.
- **Code Changes:** None (file relocation).
- **Resolved?** Yes.

## Bug 2: Form Submission Issue
- **Description:** The form submission logic was incorrect, causing notes not to be added properly.
- **Approach:** Refactored the form submission logic to properly handle the POST request and append notes to the `notes` list.
- **Code Changes:** Added a condition to check if the request method is POST, then append the note to the `notes` list.
- **Resolved?** Yes.

## Bug 3: Incorrect Method for Retrieving Form Data
- **Description:** The code was using `request.args.get()` instead of `request.form.get()` to retrieve form data from the POST request.
- **Approach:** Updated the code to use `request.form.get()` to correctly retrieve form data.
- **Code Changes:** Updated `request.args.get()` to `request.form.get()`.
- **Resolved?** Yes.

### Summary
The Note Taking Application has been successfully fixed and is now fully functional. All identified bugs have been addressed, ensuring smooth operation of the application. The codebase has been refactored and optimized to improve readability and maintainability.

