# Aaron Ciuffo - Resume

Featured Git Repositories

## Work Related Projects

### [gdrive_audit](https://github.com/txoof/gdrive_audit)

Audit ownership of all files in a Google Drive folder.

GDrive Audit produces a google sheet that shows all the files within a folder and their owners. This tool can aid google super admins migrating folders into a Google Shared Drive. Run the audit tool to verify that all items contained within the shared folder are owned by the team and are suitable for migrating into a Google Shared Drive.

Remember: When super-admins migrate a folder into a Shared Drive all ownership of the files is transferred to the organization. This is strictly a ONE WAY process and cannot be undone. If items that are meant for organization-wide consumption are migrated, the rest of the organization will lose access. Each item must be individually restored to the original owner. There is no undo.

### [insertFiles](https://github.com/txoof/insertFiles)

Quikcly insert files iles by grade-level into Student Cumulative Folders on Google Drive. This can assist in adding standardized test scores, report cards or similar documents into Student Cumulative Folders.

### [PortfolioCreator](https://github.com/txoof/portfolioCreator)

Create student cumulative folders on Google Drive using Google FileStream and student information exports from PowerSchool.

### [codesign](https://github.com/txoof/codesign)

Python3 script for signing, packaging, notarizing and stapling Apple command line binaries using altool. This script only requires Python3 and uses only standard libraries.

This script is specifically targeted at codesigning, notarizing, creating .pkg files and stapling the notarization onto commandline tools written and compiled outside of Apple Xcode. This was created specifically for notarizing and signing python tools created with PyInstaller.

As of MacOS Catalina, all distributed binaries must be signed and notarized using an apple developer account. This account costs $99 per year. Theives.

Apple's documentation for this process is ABSOLUTELY terrible. For a guide to doing this manually see Signing_and_Notarizing_HOWTO

### [IMSCC_scripts](https://github.com/txoof/IMSCC_scripts)

Extract all regular files from Learning Management Platform Common Cartridge files (IMSCC). This can help you locate individual files that are contained within an IMSCC archive downloaded from platforms such as Canvas, Brightspace, Moodle or PowerSchool Learning.

### [pdfEdit](https://github.com/txoof/pdfEdit)

Edits individual PDF reports into a single file ready for Alert Solutions in PowerSchool.

Alert Solutions can read a large PDF file containing information on multiple students and parse that file into individual emails. To distinguish one record from the next Alert Solutions looks for the following text (exactly and with absolutely no flexibility) where XXXXXX is the student number: StudentID:XXXXXX

This script searches individual MAP test results in PDF Format or the line "Student ID: XXXXXX" and replaces it with the Alert Solutions expectation and then combines the edited PDFs into a single large PDF file that Alert Solutions can use.

### [pyPDF_split](https://github.com/txoof/pyPDF_split)

Split PDFs with multiple student records into individual PDFs. This can aide in preparing PDF files for mail merges or sharing in Google Drive.

pyPDF_split searches a PDF for the string StudentID:NNNNNNN and splits the PDF into individual PDFs in a sub-folder with the StudentID embedded in the new file name.

pyPDF_split can handle student IDs in the following formats:

StudentID:123456; StudentId:123456; STUDENTID:123456; studentid:123456
upper/lower case is ignored in all cases
Student ID:123456; Student ID: 123456
pyPDF_split pairs nicely with the insertFiles and create_folders scripts.



## Hobby Projects

|             |                 |              |
|:-----------:|-----------------|--------------|
|    <img src=https://github.com/txoof/PaperPi/blob/main/documentation/images/paperpiV3.gif alt="PaperPi" width=400 /></br>[PaperPi](https://github.com/txoof/PaperPi)   | Useless Machine | Audio Sensor |
| NPR2Podcast | epdlib          | querylms     |
