# AI Automated Cover Letter Generator

This Jupyter Notebook streamlines and automates the process of generating a first-draft cover letter for job or internship applications using Python libraries and the OpenAI API.


# Features



* Automatically extracts the company name from the resume filename.
* Reads and processes job listings from images.
* Dynamically generates a personalized cover letter using your resume and job listing.
* Outputs a formatted cover letter in .docx format.
* Tracks token usage for efficient API management.


# How It Works


## Input Requirements:



* A resume in PDF format. The resume file should follow the naming format: Resume_[CompanyName].pdf. The company name will be extracted from the file name.
* A screenshot of the job listing in image format.


## Process:


### Resume Handling:



* The script uses the PyPDF2 library to read and store the content of your resume. The company name is dynamically extracted from the filename for inclusion in the cover letter.


### Job Listing Handling:



* The pytesseract library is used to extract text from the provided job listing image.


### Cover Letter Generation:



* The script dynamically crafts a tailored cover letter using the OpenAI API, integrating the details from the job listing and your resume.
* A predefined prompt ensures the cover letter:
    * Follows a professional format.
    * Includes essential details like experience, education, and skills.
    * Is customized to the job position.


## Output:



* A docx file containing the generated cover letter is saved in the same folder as your resume.
* The script also outputs the number of input and output tokens used, helping you track your OpenAI API usage.


# Disclaimer



* This script generates a first draft of the cover letter. Always review and refine it for accuracy and personalization before submitting.
* The script provides token usage stats for cost tracking.
* The crafted prompt is embedded in the script but not shared in the repository for security reasons.
* You would need your own OpenAI API key to run this script
