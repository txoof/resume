# Aaron Ciuffo - Project Summary

*Featured Professional and Personal Repositories*

This selection of repositories contains some of my best work. There are great examples of complete projects, libraries written to support projects, problem solving and great documentation.
* [Work Related Projects](#work-related-projects): Software created to solve problems and patch together systems.
* [Hobby Projects](#hobby-projects): Projects and software created for the fun and pleasure of creating new things!

## Work Related Projects

### [PowerSchool PowerQuery](https://github.com/txoof/PowerQuery)

PowerSchool Student Information System (SIS) PowerQuery PL/SQL plugins for integrating course, teacher, student and parent data into D2L/Brightspace Learning Management System (LMS). There is no off-the-shelf integration between these products. A customized solution is required to maintain accurate synchronization of these two systems. This synchronization occurs regularly and ensures that staff, parents and students are connected to the appropriate classes and any changes to student schedules such as a schedule or class change are managed.

The queries are written in a combination of Oracle SQL and managed through XML documents. Once packaged and installed on the SIS server, the plugin can be accessed through automation processes and set to synchronize comma separated value (CSV) data to the D2l/Brightspace instance in the cloud. 

### [gdrive_audit](https://github.com/txoof/gdrive_audit)

Audit ownership of all files in a Google Drive folder.

GDrive Audit produces a google sheet that shows all the files within a folder and their owners. This tool can aid google super admins migrating folders into a Google Shared Drive. Run the audit tool to verify that all items contained within the shared folder are owned by the team and are suitable for migrating into a Google Shared Drive.

Remember: When super-admins migrate a folder into a Shared Drive, all ownership of the files is transferred to the organization. This is strictly a ONE WAY process and cannot be undone. If items that are meant for organization-wide consumption are migrated, the rest of the organization may lose access. Each item must be individually restored to the original owner. There is no undo. **Migrate with caution!**

### [insertFiles](https://github.com/txoof/insertFiles)

Quikcly insert files by grade-level into Student Cumulative Folders on Google Drive. This can assist in adding standardized test scores, report cards or similar documents into Student Cumulative Folders.

### [PortfolioCreator](https://github.com/txoof/portfolioCreator)

Create student cumulative folders on Google Drive using Google FileStream and student information exports from PowerSchool.

### [calendar_csv](https://github.com/txoof/calendar_csv)

Python script for generating files suitable for import into Google Calendar based on .csv schedule files for N-day rotating block schedules for schools. This script will produce one CSV for each unique event as well as a CSV for each day in the block rotation.

If your schedule has "Block A, Block B, Block C, Lunch, Break 1, Break 2" seven CSV files will be produced, one for each event in the rotation: e.g. Block A, Block B, Block C, lunch, breaks. Each file produced will contain all of the calendar events for all days that match that event.

### [codesign](https://github.com/txoof/codesign)

Python3 script for signing, packaging, notarizing and stapling Apple command line binaries using altool. This script only requires Python3 and uses only standard libraries.

This script is specifically targeted at codesigning, notarizing, creating .pkg files and stapling the notarization onto commandline tools written and compiled outside of Apple Xcode. This was created specifically for notarizing and signing python tools created with PyInstaller.

As of MacOS Catalina, all distributed binaries must be signed and notarized using an apple developer account. This account costs $99 per year. .

Apple's documentation for this process is ABSOLUTELY terrible. For a guide to doing this manually see [Signing_and_Notarizing_HOWTO](https://github.com/txoof/codesign/blob/main/Signing_and_Notarizing_HOWTO.md)

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

### [PaperPi](https://github.com/txoof/PaperPi#paperpi-v3-)

PaperPi is a lovely, quiet, *slow internet* e-Paper radio. There are no loud colors, no busy animations, just a lovely selection of the information you want without buzz and distraction. PaperPi rotates through your choice of plugin screens at the pace you choose.

![PaperPi Video](https://github.com/txoof/PaperPi/blob/main/documentation/images/paperpiV3.gif)

### [ItsyBitsy Useless Machine](https://github.com/txoof/Useless_Machine)

***Absolutely Useless, Completely Necessary***

It's pretty useless. It defies logic and your will. It's a machine that has exactly one purpose, to turn its self off. For something so absolutely useless, why is it so entertaining?

![Usless Machine Animation](https://github.com/txoof/Useless_Machine/blob/main/Useless_Machine.gif)

### [Audio Sensor irBlaster](https://github.com/txoof/audioSensor)

 Let's face it: nobody knows how to operate your stereo receiver. Your kids, husband, sister-in-law all just want to start music playing and have sound come out of the speakers. It should *just work*, not be an exercise in frustrated button mashing.

It's a mystery which remote turns on the stereo. It's an even bigger mystery which button switches it so Spotify or the CD player plays. The irBlaster helps solve this problem by listening to two channels such as a CD Player and Media PC with Spotify, Movies, etc.

The irBlaster listens to the line-level audio over the RCA jacks. When audio traffic is detected on one of the channels, it sends a POWER ON Infrared (IR) code to the receiver. After a few seconds wait for the reciever to power up, the irBlaster then sends the IR code for the active input. When the audio traffic stops, the irBlasters sends the POWER OFF IR code to the receiver.
![irBlaster Image](https://github.com/txoof/audioSensor/blob/master/irBlaster.jpg)

### [Raspberry Pi Case](https://github.com/txoof/pi4_case)

Customizable, laser cut case for Raspberry Pi 3 and 4 written in OpenSCAD. This case has room for a Pi and HiFi Berry DAC+ HAT. The case provides access to all Pi IO ports as well as the RCA connectors and GPIO pins on the HiFi Berry.

| | |
|-|-|
|<img src="https://github.com/txoof/pi4_case/blob/master/pi4_case_back.png" alt="pi4 case render" width="400"/>|<img src="https://github.com/txoof/pi4_case/blob/master/pi_4_back.jpg" alt="pi4 case photo" width="400"/>

### [Ansible](https://github.com/txoof/ansible)

Ansible playbooks for configuring, deploying and managing Raspberry Pi devices. 

These playbooks make it easy to spin up a Raspberry Pi from a scratch image and install relevant tools and setup development environments.
### [epdlib](https://github.com/txoof/epdlib)

EpdLib is a library for creating dynamically scaled screen layouts for frame-buffered devices such as e-paper/e-ink displays. Complex layouts are created by defining image, drawing or text blocks. By Using epdlib blocks makes it trivial to develop for different display resolutions as layouts are aware of their resolution and scale the blocks dynamically to match the available area at a given resolution.

#### Example of scaled layout

| | |
|-|-|
|![500x500 Layout](https://github.com/txoof/epdlib/blob/master/docs/weather_5x5.png)<br/> 500x500 Layout| ![300x200 Layout](https://github.com/txoof/epdlib/blob/master/docs/weather_3x2.png) <br/> 300x200 Layout|

### [QueryLMS](https://github.com/txoof/querylms)

Manage queries to an Logitech Media Server for a single player instance. A QueryLMS object can be used to query server or player status information and control an LMS player.

This is based heavily on the [LMSQuery](https://github.com/roberteinhaus/lmsquery) library and reuses significant portions of the code.
